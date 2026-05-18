function initAdmin() {
  const user = Session.get();

  document.getElementById('admin-user-name').textContent = user.name;
  document.getElementById('admin-user-role').textContent = 'Administrator';

  document.querySelectorAll('#admin-app .nav-item').forEach(link => {
    link.addEventListener('click', e => {
      e.preventDefault();
      const page = link.dataset.page;
      navigateTo(page, 'admin');

      const loaders = {
        dashboard: renderAdminDashboard,
        members: renderAdminMembers,
        trainers: renderAdminTrainers,
        subscriptions: renderAdminSubs,
        attendance: renderAdminAttendance,
        payments: renderAdminPayments
      };

      if (loaders[page]) loaders[page]();
    });
  });
  
  navigateTo('dashboard', 'admin');
  renderAdminDashboard();
}
### Explanation : 
This function initializes the admin dashboard after login.
It retrieves the logged-in user from the session and displays the admin’s name and role.
It also controls navigation between different sections of the system such as dashboard, members, trainers, attendance, and payments.

. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .

const member = DB.insert('members', {
  name,
  age,
  phone,
  membership_type: plan,
  start_date: start,
  end_date: end,
  status
});

const nextId = DB.getNextLoginId('member');
const password = DB.getDefaultPassword(String(nextId), 'member');

DB.insert('users', {
  login_id: String(nextId),
  role: 'member',
  name,
  linked_id: member.id,
  password
});
### Explanation : 
This code adds a new gym member into the system. it stores the member’s personal and membership details in the database first , then
Then it automatically creates a login account for the member with a generated ID and password.

. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 

const dup = DB.getAll('attendance').find(
  a => a.member_id === mid && a.check_in_date === date
);

if (dup) {
  toast('Already checked in on this date.', 'err');
  return;
}

DB.insert('attendance', {
  member_id: mid,
  check_in_date: date,
  check_in_time: time
});
### Explanation : 
This function records gym attendance Before adding a new check-in
it checks if the member has already checked in on the same date If a duplicate record exists
it stops the operation and shows an error message
