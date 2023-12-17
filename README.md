### Project Report: Enhancing Functionality and Overcoming Challenges
In this project, I developed a comprehensive system comprising various files and functionalities to 
manage staff members, their activities, and time-related operations. The project involves the creation 
of several files, each serving specific purposes to ensure a seamless operation of the system.
#### File Structure and Class Hierarchy
I initiated the project by creating a file named `class.js`, which houses distinct classes: “Employee”, 
“Staff_Member”, and “Delivery_Driver”. The latter two classes 
inherit properties and behaviors from the `Employee` class, facilitating a streamlined structure for 
managing different staff roles.
What this class containing are as shown in screenshot, picture, email, time the staff being out and 
status of staff. Additionally, the class contain a function called “StaffMemberIsLate” which triggers a 
toast notification if a member is late, providing comprehensive information about the tardiness.
The Delivery_driver class contains following properties as vehicle, telephone, deliver Adress and 
return Time. Additionally, the class contain a function called “deliveryDriverIsLate” which triggers a 
toast notification if the delivery driver is late.
The “Clock.js” file was designed to acquire and manage time-related data such as date, hour, and 
other relevant information. This module is crucial for various time-sensitive operations within the 
system.
It contain a function called “digitalClock”, to retrieve and dislay the current time (hours, minutes, 
seconds). It formats the time values to always show two digits and updates the HTML elements with 
the corresponding classes to reflect the current time. The “setInterval” method calls “digitClock”
every second to keep the time updated in real-time. Additionally, it retrieves the current data and 
displayes it in a specific format, updating the respective HTML elements with day, date, month and 
year information.
#### Delivery Management
Another integral component is the “Delivery.js” file, housing functions essential for managing 
deliveries. Functions like:
1- “deliveryDriverIsLate(driverId): this function checks if a delivery driver is late based on their 
return time. It continuously checks and triggers a toast notification if the driver is overdue.
2- “addDelivery”: validates input data for a new delivery, creates a table row displaying the 
details, highlights the added row, creates a new Delivery Driver object, triggers the 
“deliveryDriverIsLate” function for the added driver, and clears input fields after successful 
addition.
3- “validateDelivery”: validate the input criteria for a delivery such as phone number length. 
Presence of name, surname, address, and return date.
4- “deliveryClear”: asks for confirmation before removing a delivery. If confirmed, it empties the 
content of the highlighted delivery row. Otherwise, it removes the highlighting from the row.
#### StaffTabell for API Integration
“StaffTabell” js file defines an asynchronous function “staffUser()” that fetches data from the 
“randomuser.me”’s API to retrieve details of five staff members. It creates instances of the 
“Staff_Member” class using the fetched data and populates an HTML table with staff information like 
name, email, and images.
Additionally, it includes functionalities for:
• Highlighting rows in the table upon click.
• Converting time into the correct format.
• Handling staff “out” actions, setting out times, expected return times, and durations.
• Managing staff “in” actions to clear cells and rest staff status.
• Generating toast notifications for late staff members based on their expected return time.
#### HTML File 
The HTML serves as a dashboard for managing staff members, deliveries, and schedules see figure 6
down below (contain the first page of the Html code and the rest of you can check when you open 
the web application). It includes several sections:
• Navbar: Contains navigation links for Dashboard, inventory, and orders, with dropdown
menus for specific actions.
• Header Section: displays the logo and a title for the reception management dashboard.
• Staff table section: show a table of staff members with details like name, surname, email, 
status, clock-in/out times, and expected return times. Buttons for clocking in and out are 
included.
• Toast notifications: alerts for late staff members, triggered with relevant information about 
the latte employee.
• Schedule Delivery Section: enables scheduling deliveries with fields for vehicle type,
recipient’s name, surname, telephone, delivery address, and return time. 
• Delivery Board Section: Displays a table for delivery drivers with columns for vehicle, name, 
surname, telephone, delivery address, and return time. Also includes a button to clear 
deliveries.
#### Challenges Faced and Solutions Implemented
During the project, I encountered several challenges that required troubleshooting and innovative 
solutions. These challenges included difficulties in populating tables with data, issues with API 
requests due to missing file linking, malfunctioning time formatting, and problems with toast 
notifications.
The resolution process involved meticulous debugging, such as rectifying file linking errors, 
restructuring code classes to streamline data population, and revising the toast notification system. 
Utilizing relative positioning and changing its trigger to a button significantly contributed to resolving 
the toast display issue. Additionally, optimizing the design in Bootstrap required numerous iterations 
and class modifications to achieve the desired layout and functionality.
Overall, the project entailed comprehensive development and problem-solving, resulting in a robust 
system for staff management and time-related operations.
This endeavor provided invaluable experience in software development, debugging, and the 
utilization of various technologies to create an efficient and user-friendly system
