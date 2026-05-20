This is the skeletal demo for the gym managment system + UI screenshots : 
User opens login page
User enters ID and password
System redirects based on role (Admin / Trainer / Member)
<img width="1919" height="1029" alt="Image" src="https://github.com/user-attachments/assets/ffefc755-03b0-46d1-ab61-f333157fe15d" />

*If the user log in as a trainer : 
System shows trainer dashboard
<img width="1917" height="1027" alt="Image" src="https://github.com/user-attachments/assets/a57fd273-d226-490e-bafb-9d6a91c630ad" />

Trainer sees only assigned members
<img width="1919" height="1027" alt="Image" src="https://github.com/user-attachments/assets/3607137c-360e-48b2-874b-a79229e3f1f5" />

Trainer can see the attendence of the members + the user can check in members 
<img width="1919" height="1029" alt="Image" src="https://github.com/user-attachments/assets/52e583a8-2d8d-4b2e-9f5c-ef5f42843120" />
<img width="480" height="316" alt="Image" src="https://github.com/user-attachments/assets/346b7787-b487-4d16-9bf1-ce0dac3f3d0d" />
<img width="1919" height="1027" alt="Image" src="https://github.com/user-attachments/assets/63c0f7cf-4682-4161-8beb-160ebc6001c3" />

Trainer can see the members that paid , the amount , the date of payment , the statues , and the discription(monthly/3months/yearly)
<img width="1917" height="1027" alt="Image" src="https://github.com/user-attachments/assets/28b343cd-91ee-429a-a0f1-cc9d78754ad8" />

*if the user log in as a member
The user sees their personal profile information.
The system displays:
Member name
Phone number
Membership type
Membership status
Subscription expiry date
The user can only view their own information.
<img width="1919" height="1031" alt="Image" src="https://github.com/user-attachments/assets/e06cd849-0245-4701-be53-26f9f5d25cd7" />

If The user opens the Subscription section.
The system displays:
Current membership plan (monthly / 3-month / yearly)
Start date
End date
Subscription status (active / expired)
The user cannot modify subscription details.
<img width="1919" height="1029" alt="Image" src="https://github.com/user-attachments/assets/7be12cbf-da43-4d5c-9ac6-59da719918c1" />

If The user opens the Attendance page.
The system displays all recorded check-ins for that member only.
The user can view:
Check-in dates
Check-in times
If the member did not attend on a certain day:
No attendance record is shown for that date
The member is considered absent by the system state
<img width="1919" height="1027" alt="Image" src="https://github.com/user-attachments/assets/9687d114-1fc2-4ac1-95c8-40b535bdc3df" />

If The user opens the Payments section.
The system displays payment history for that member only.
The user can view:
Payment amount
Payment date
Payment status (paid/unpaid)
Payment description
The user cannot edit payment records.
<img width="1919" height="1029" alt="Image" src="https://github.com/user-attachments/assets/211e7578-5491-4610-a888-6e1593642139" />

*If the user log in as an Admin : 
The Admin sees an overview dashboard containing gym statistics.
The system displays:
Total members
Total trainers
Active memberships
Attendance and payment summaries
The Admin can navigate through different management sections using the sidebar.
<img width="1917" height="1029" alt="Image" src="https://github.com/user-attachments/assets/ad5c4e8d-c85e-47fb-a5f7-281fa7e4f6e0" />

 If The Admin opens the Members section.
The system displays a table of all registered members.
The admin can:
Add a new member
<img width="1917" height="1029" alt="Image" src="https://github.com/user-attachments/assets/a9235946-8c2c-460f-b4b0-e375caf67d34" />


Edit member information
<img width="1917" height="1029" alt="Image" src="https://github.com/user-attachments/assets/8a89adfc-e647-4271-8945-1c12c25a2c0b" />


Delete a member
<img width="447" height="152" alt="Image" src="https://github.com/user-attachments/assets/df4d6434-6324-40f6-827f-a1668aa45692" />


Search members by name or phone number
<img width="329" height="85" alt="Image" src="https://github.com/user-attachments/assets/9de52993-ec97-4eef-af81-1f9214b103e2" />


The system stores all changes in the database layer.
<img width="1916" height="1029" alt="Image" src="https://github.com/user-attachments/assets/7c7a5fe3-1ee7-4521-9ff7-a414eda7fbcd" />


If The Admin opens the Trainers section.
The system displays all trainers registered in the system.
The Admin can:
Add trainers
<img width="1919" height="1031" alt="Image" src="https://github.com/user-attachments/assets/2640daa0-22a8-4661-a8ca-d097efdaf2fc" />


Edit trainer details
<img width="1917" height="1029" alt="Image" src="https://github.com/user-attachments/assets/54e7d0ef-0d89-4d98-aefa-b339afb8fe93" />


Delete trainers
<img width="445" height="152" alt="Image" src="https://github.com/user-attachments/assets/7979609e-41ca-49ea-ae81-1ffa0346e7f5" />


Assign members to trainers
<img width="480" height="312" alt="Image" src="https://github.com/user-attachments/assets/f02b3e9a-f6cf-4c91-a2fa-bda485bf7701" />


The system updates trainer assignments dynamically.
<img width="1916" height="1029" alt="Image" src="https://github.com/user-attachments/assets/7c7a5fe3-1ee7-4521-9ff7-a414eda7fbcd" />

If The user opens the Payments or Subscription section:
The system displays:
Membership plans
Payment amounts
Subscription status
Expiry dates
<img width="1919" height="1029" alt="Image" src="https://github.com/user-attachments/assets/c9fb7639-bee5-465a-a840-ebeb08530b72" />


The admin can:
Add a new subscription
<img width="1919" height="1029" alt="Image" src="https://github.com/user-attachments/assets/542e5b72-a066-4a92-a3c5-7087b44b0986" />

If The admin opens the Attendance section:
The system displays attendance records for all members.
<img width="1919" height="1027" alt="Image" src="https://github.com/user-attachments/assets/85a16dae-6665-4a39-bcda-7ca4c59458b8" />


The admin can:
Filter attendance by date
Monitor check-in activity
<img width="1917" height="1027" alt="Image" src="https://github.com/user-attachments/assets/89b7714d-9d77-47bb-80fa-ff04b48a87cb" />



And the admin can check in members : 
<img width="480" height="309" alt="Image" src="https://github.com/user-attachments/assets/d51429fd-727d-4576-9291-f82a3887bfb4" />





