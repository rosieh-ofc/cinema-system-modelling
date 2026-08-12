# DATABASE FOR CINEMA MOVIE

### General Description
VVI Cinema is the most famous cinema in Bandung. This cinema requires an app for booking, payment, and daily transaction recording. The app can help streamline VVI Cinema's business processes.

---

### Business Rules Details
1. System Users: There are two types of users in this application, namely admin and member. Admin is an employee who is responsible for managing transactions, film schedules, and customer service. Members can purchase tickets online or offline, while non-members can only purchase tickets offline at the cinema ticket counter.
2. Account Management: Each member has an account with information such as name, email, phone number, and password. Admin data includes address, salary, and branch data.
3. Purchase Term and Discounts: Member may purchase one or more tickets. DIscounts may be awarded based on specific events, membership status, or payment methods.
4. Transaction and Payment Mechanism: Each purchase is recorded with the purchase number, purchase date, purchase time, discount, total payment, payment method, status (Unpaid/Paid/Cancelled). For non-member customers, purchases can only be made offline at the counter and customer data will not be saved, but non-member purchase transactions will be represented by the data of the admin who handles the transaction.
5. Ticket Details and Purchaser Validation: This page displays detailed information about the ticket purchased. Ticket contain information such as the ticket number, purchaser details (if the purchaser is a member). Otherwise, the purchaser details are left blank if the purchase is made by a non-member, the schedule, studio details and seat number, the film being shown, and the ticket price.
6. FIlm Management and Scheduling: Films have details such as title, duration, genre, age rating, and showtime. Each showtime is only valid for one film from one studio at a certain time. Each film can be grouped into several genres. The showtime consists of film data, studio data, cinmea branch data, showtime, start time, end time, film format(2D/3D/IMAX/4DX).
7. Branch and Studio Facilities: Each branch has information on the branch name, address, city, number of studios, and operating hours. Each studio has a studio number, capacity, and studio type (2D, 3D, IMAX, VIP, etc.).
8. Seat Management: Each seat in the studio has a seat number, seat type (Regular/VIP/Sofa/Recliner), and status (available/reserved/damaged). Each seat can only be reserved by one ticket at a specific showtime and cannot be used by more than one buyer at the same time.

---

## Conceptual Modelling
### Entities and Attributes


| No. | Entity Name | Entity Type | Description |
| :---: | :---: | :---: | :---: |
| **1.** | **Member** | Strong Entity | **Customers are parties who make purchases of goods or services offered by a company.**<br><br>Customers can be individuals or companies/organizations. |
| **2.** | **Admin** | Strong Entity | Cinema employees or staff whose job is to manage transaction data, film schedules, studio operations, and serve ticket purchases at the physical counter. |
| **3.** | **Branch** | Strong Entity | The physical location or place of a VVI cinema that operates in a particular city and has facilities such as several studios and administrative staff. |
| **4.** | **Purchase** | Strong Entity | A valid transaction record or payment receipt for the purchase of one or more tickets by a customer (member or non-member). |
| **5.** | **Studio** | Strong Entity | A film screening room located within a cinema branch, which has a certain capacity and a certain type of media projection technology. |
| **6.** | **Chair** | Strong Entity | Represents a physical seating asset, where each seat has its own unique Seat ID within the system (independent of the studio number for its primary identification), and is related to the Studio entity. |
| **7.** | **Film** | Strong Entity | Audio-visual works of art (wide screen) registered in the system for screening in cinemas, complete with information on duration, age rating, and genre. |
| **8.** | **Broadcast Schedule** | Strong Entity | A specific screening session of a film at a specific studio and branch on a specified date and time. |
| **9.** | **Tickets** | Strong Entity | Proof of physical or electronic transactions that have their own unique code (such as Ticket ID or Serial Number), which gives viewers access rights to watch films at certain showtimes and seat numbers. |
| **10.** | **Discount** | Strong Entitiy | Active discount or promo programs that can be applied to purchase transactions based on criteria or conditions certain. |

