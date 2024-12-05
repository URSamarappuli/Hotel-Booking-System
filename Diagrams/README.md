# Key Features
    * Room Booking: Enables receptionists to check room availability and book rooms for customers.
    * Customer Management: Handles customer check-ins, check-outs, and billing information.
    * Inventory Management: Allows managers to track hotel inventory status and make purchases as needed.
    * Billing System: Generates bills for customers based on their stay and other services used.
    * Feedback Collection: Provides a way for receptionists to collect feedback from customers.

# Key Entities

    Manager:
        + Responsible for managing hotel staff, purchasing inventory, and recording complaints.
        + Attributes: Name, ID, Phone Number, Location.
        + Key Methods: PurchaseInventory(), RecordComplaints(), ManageStaff().

    Receptionist:
        + Handles room availability checks, room bookings, bill generation, and feedback collection.
        + Attributes: ID, Name, Telephone Number, Address.
        + Key Methods: CheckRoomAvailability(), BookRoom(), GenerateBill(), AcceptCustomerFeedback().

    Customer:
        + Represents individuals staying in the hotel.
        + Attributes: ID, Name, Telephone Number, Address, Room Number.
        + Key Methods: CheckIn(), CheckOut(), PaysBill().

    Rooms:
        + Represents the rooms available in the hotel.
        + Attributes: Room Number, Location.

    Inventory:
        + Tracks the type and status of the hotel's inventory.
        + Attributes: Type, Status.

    Bill:
        + Stores billing information for customers.
        + Attributes: Bill Number, Customer Name.

# System Relationships
    * Managers oversee inventory and complaints.
    * Receptionists interact with customers for room bookings and billing.
    * Customers are assigned rooms and billed upon checkout.