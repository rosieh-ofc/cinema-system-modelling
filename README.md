# DATABASE FOR CINEMA MOVIE

### General Description
VVI Cinema is the most famous cinema in Bandung. This cinema requires an app for booking, payment, and daily transaction recording. The app can help streamline VVI Cinema's business processes.

### Business Rules Details
1. System Users: There are two types of users in this application, namely admin and member. Admin is an employee who is responsible for managing transactions, film schedules, and customer service. Members can purchase tickets online or offline, while non-members can only purchase tickets offline at the cinema ticket counter.
2. Account Management: Each member has an account with information such as name, email, phone number, and password. Admin data includes address, salary, and branch data.
3. Purchase Term and Discounts: Member may purchase one or more tickets. DIscounts may be awarded based on specific events, membership status, or payment methods.
4. Transaction and Payment Mechanism: Each purchase is recorded with the purchase number, purchase date, purchase time, discount, total payment, payment method, status (Unpaid/Paid/Cancelled). For non-member customers, purchases can only be made offline at the counter and customer data will not be saved, but non-member purchase transactions will be represented by the data of the admin who handles the transaction.
5. Ticket Details and Purchaser Validation: This page displays detailed information about the ticket purchased. Ticket contain information such as the ticket number, purchaser details (if the purchaser is a member). Otherwise, the purchaser details are left blank if the purchase is made by a non-member, the schedule, studio details and seat number, the film being shown, and the ticket price.
6. FIlm Management and Scheduling: Films have details such as title, duration, genre, age rating, and showtime. Each showtime is only valid for one film from one studio at a certain time. Each film can be grouped into several genres. The showtime consists of film data, studio data, cinmea branch data, showtime, start time, end time, film format(2D/3D/IMAX/4DX).
7. Branch and Studio Facilities: Each branch has information on the branch name, address, city, number of studios, and operating hours. Each studio has a studio number, capacity, and studio type (2D, 3D, IMAX, VIP, etc.).
8. Seat Management: Each seat in the studio has a seat number, seat type (Regular/VIP/Sofa/Recliner), and status (available/reserved/damaged). Each seat can only be reserved by one ticket at a specific showtime and cannot be used by more than one buyer at the same time.
