CIS 4374 Semester Project: Smart Parking Platform

1. Introduction:  
   1. Purpose: The Purpose of this document is to plan to plan out and manage a software that will allow drivers to locate, reserve, and pay for parking in real time through both web and mobile platforms.   
        
   2. Scope: The scope of this project currently includes: Real-time view of parking spaces that are available through an interactive map, Digital payment processing, Notifications and alert systems for users.  
2. Overall Description:  
* Users: Customers seeking parking, parking administrators.  
* System Environment: Web-based and mobile application  
* Constraints: Must be able to run on basic hardware and require some form of authentication. Likely user and password.  
* Assumptions: Application will have access to internet  
3. Functional Requirements  
* FR1: System needs to allow users to login and register in a secure manner.  
* FR2: System should allow users to add items like car license plates for ease of access.  
* FR3: System should should require no more than 5 fields per parking registration  
4. Non-Functional Requirements  
* NFR1: System shall be able to serve up to 100 concurrent users at any given time  
* NFR2: System will auto update every 10 seconds  
* NFR3: The system will have uninterrupted downtime at a rate of 99 percent

Use Cases:

UC1:   
Actor: Parking customer

Goal: Create an account 

User Story: As a parking customer, I want to create an account.

UC2:   
Actor: Parking customer

Goal:View nearby parking spaces and garages on a map with current availability. 

User Story: I want to see a live map of available parking so that I can find somewhere to park. 

UC3:   
Actor: Parking customer

Goal: Find parking near a specific address

User Story: I want to search for parking near a destination so that I can plan where to park before arriving. 

UC4:  
Actor: Parking customer

Goal: Filter parking by price, distance, and accessibility

User Story: I want to filter parking options so that I can find a space that meets my needs. 

UC5:   
Actor: Parking customer

Goal: Look at a parking locations rates and availability 

User Story: I want to view parking details so that I can decide whether a location is suitable 

UC6:   
Actor: Parking customer

Goal: Book an available parking space for a selected date, start time, and duration. 

User Story: I want to reserve a parking space so that I have a confirmed place to park when I arrive. 

UC7:   
Actor: Parking customer

Goal: Pay for a parking reservation and receive confirmation of payment. 

User Story: I want to pay for my reservation through the website or mobile application 

UC8:   
Actor: Parking customer

Goal: Change reservation details or cancel a booking 

User Story: I want to modify or cancel my reservation so that I can adjust my parking arrangements when my plans change. 

UC9:   
Actor: Parking customer

Goal: Obtain directions to the reserved parking location. 

User Story: I want directions to my reserved parking location so that I can reach the correct space.

UC10:   
Actor: Parking customer

Goal: Receive booking confirmations, upcoming reservation reminders, and parking expiration alerts. 

User Story: I want timely notifications about my reservation so that I can arrive on time and avoid overstaying. 

UC11:   
Actor: Parking customer

Goal: Extend an active parking session.

User Story: I want to extend my parking session and pay any additional charges so that I can stay longer without having to return to my vehicle. 

UC12:   
Actor: Parking admin

Goal: Add, update, or deactivate parking garages, lots, and individual spaces. 

User Story: I want to manage parking locations and space details so that customers see accurate listings and booking options. 

UC13:   
Actor: Parking admin

Goal: Configure parking rates, operating hours, reservation limits, and cancellation policies. 

User Story: I want to manage pricing and booking rules so that reservations follow the requirements of each parking location. 

UC14:   
Actor: Parking admin

Goal: Monitor live occupancy and mark spaces unavailable for maintenance, closures, and other needs. 

User Story:I want to monitor occupancy and update space availability so that customers can only book spaces that are ready for use. 

UC15:   
Actor: Parking admin

Goal: Review occupancy, reservations, cancellations, and revenue over a selected period. 

User Story: I want to view operational reports so that I can evaluate parking demand and make informed management decisions. 

