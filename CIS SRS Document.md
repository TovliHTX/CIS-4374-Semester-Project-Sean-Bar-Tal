CIS 4374 Semester Project: Smart Parking Platform

1. Introduction:  
1.1 Purpose: This Software Requirements Specification defines the functional and nonfunctional requirements for the Smart Parking Platform. The platform will allow drivers to locate, reserve, navigate to, and pay for parking through web and mobile applications. It will also provide parking operators with tools to manage parking locations, availability, pricing, reservations, and operational reports.
        
1.2 Scope:
The Smart Parking Platform will provide:

Secure user registration and authentication
User profiles and saved vehicle information
Real-time parking availability
An interactive map of parking garages, lots, and spaces
Destination search and filters for price, distance, accessibility, and availability
Parking reservations, modifications, cancellations, and extensions
Digital payment processing, receipts, and eligible refunds
Navigation assistance through an external mapping service
Reservation confirmations, reminders, and expiration alerts
An administrative dashboard for parking operators
Occupancy, reservation, cancellation, and revenue reports
The platform will be available through web and mobile interfaces and will integrate with external mapping, payment, and notification services.

Unless approved through the project change-control process, the following items are outside the current scope:

Construction or physical operation of parking facilities
Manufacturing or installation of parking sensors
Cash payment processing
Parking citation issuance or city enforcement
Autonomous vehicle parking
Ownership of third-party mapping or payment systems


2. Overall Description:  
2.1 Product Perspective
The Smart Parking Platform is a new software system consisting of web and mobile applications supported by backend services and a database. The customer-facing applications will communicate with the backend through secured APIs. The backend will integrate with external mapping, payment, and notification services.

2.2 User Classes
Parking Customer: Creates an account, manages vehicles, locates parking, makes payments, manages reservations, receives notifications, and views receipts.
Parking Administrator: Manages parking locations, spaces, pricing, availability, reservation rules, and operational reports.
System Administrator: Manages access, monitors system health, and supports security and recovery activities.
Finance and Billing Personnel: Reviews transactions, refunds, receipts, and revenue records.
External Stakeholders: City transportation representatives and third-party mapping, payment, and notification providers.

2.3 Operating Environment
Responsive web application supported by current desktop and mobile browsers
Mobile application for commonly used mobile operating systems
Internet-connected application and database services
Third-party mapping, payment, and notification APIs

2.4 Constraints
The project must be planned and documented within the fixed semester timeline.
The platform depends on third-party mapping, payment, and notification services.
The platform must comply with applicable security, privacy, payment, and city requirements.
Protected customer and administrative functions must require authenticated, role-based access.
External provider outages or API changes may limit mapping, payment, or notification functions.

2.5 Assumptions and Dependencies
Users will have internet access and location services when using location-based features.
Parking operators will provide accurate location, space, pricing, and operating-hour information.
Availability data will be received from operator systems, approved data feeds, or simulated sources during development.
Payment, mapping, and notification providers will supply working APIs or sandbox environments.
Users will provide valid account, vehicle, and payment information.

3. Functional Requirements
FR-01: The system shall allow a customer to create an account using no more than five required registration fields.
FR-02: The system shall validate required registration fields and prevent duplicate accounts using the same verified email address.
FR-03: The system shall allow registered users to sign in and sign out securely.
FR-04: The system shall allow customers to add, update, and remove saved vehicle information, including license plate information.
FR-05: The system shall restrict administrative functions to authorized administrator accounts.
FR-06: The system shall display nearby parking garages, lots, or spaces on an interactive map.
FR-07: The system shall display the current availability status of each listed parking location.
FR-08: The system shall allow customers to search for parking near an entered address or selected destination.
FR-09: The system shall allow customers to filter parking results by price, distance, accessibility, and availability.
FR-10: The system shall display parking details, including address, rates, operating hours, availability, accessibility information, and applicable reservation rules.
FR-11: The system shall allow a customer to request a reservation by selecting a parking location, date, start time, and duration.
FR-12: The system shall verify availability immediately before confirming a reservation.
FR-13: The system shall prevent overlapping confirmed reservations for the same reservable space and time period.
FR-14: The system shall generate a unique reservation confirmation after a successful booking.
FR-15: The system shall allow customers to view current and previous reservations.
FR-16: The system shall allow customers to modify or cancel eligible reservations according to the location’s policies.
FR-17: The system shall allow customers to extend an active parking session when availability and parking rules permit.
FR-18: The system shall calculate and display any additional charge before confirming a parking-session extension.
FR-19: The system shall calculate the total reservation price, including applicable rates, fees, and taxes, before payment.
FR-20: The system shall process digital payments through an approved third-party payment provider.
FR-21: The system shall confirm a paid reservation only after receiving a successful payment result.
FR-22: The system shall provide a receipt containing the reservation identifier, parking location, date, time, and amount paid.
FR-23: The system shall process eligible refunds according to the applicable cancellation policy and record the transaction status.
FR-24: The system shall provide directions to a selected or reserved parking location through an external mapping service.
FR-25: The system shall send reservation confirmations, upcoming-reservation reminders, and parking-expiration alerts and allow customers to manage available notification preferences.
FR-26: The system shall provide an administrative dashboard and allow authorized administrators to add, update, and deactivate parking garages, lots, and spaces.
FR-27: The system shall allow administrators to configure rates, operating hours, reservation limits, and cancellation policies.
FR-28: The system shall allow administrators to view current occupancy, mark spaces unavailable for maintenance or closures, and prevent customers from reserving unavailable spaces.
FR-29: The system shall allow authorized users to generate and export occupancy, reservation, cancellation, and revenue reports for a selected period.

4. Nonfunctional Requirements
NFR-01: The system shall support at least 100 concurrent authenticated users during planned performance testing.
NFR-02: The system shall refresh displayed parking-availability data at least once every 10 seconds while a customer is viewing the map.
NFR-03: Under normal operating conditions, 95% of interactive requests shall return a response within three seconds, excluding delays controlled by third-party services.
NFR-04: The production platform shall maintain at least 99% monthly availability, excluding scheduled maintenance and verified third-party outages.
NFR-05: Reservation and payment operations shall not create duplicate confirmed reservations when a user retries a request.
NFR-06: The system shall preserve confirmed reservation and transaction records if a customer application disconnects.
NFR-07: The system shall encrypt network communication using an approved secure transport protocol.
NFR-08: The system shall store passwords using a salted, one-way password-hashing method.
NFR-09: The system shall enforce role-based access control for customer, administrator, system-administration, and billing functions.
NFR-10: The system shall not store full payment-card details; the approved payment provider shall handle payment information.
NFR-11: Core customer and administrative workflows shall use accessible labels, sufficient color contrast, and keyboard navigation where supported.
NFR-12: The web application shall support the two most recent major versions of commonly used modern browsers during acceptance testing.

5. Use Cases:

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

