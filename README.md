# Designing a Parking Lot
## ID:209076003

<div>
<p>
  <h2>Use Case Diagram</h2>
  <ul>
    <li><a href="#">Admin:</a> Mainly responsible for adding and modifying parking floors, parking spots, entrance, and exit panels, adding/removing parking attendants, etc.</li>
    <li><a href="#">Customer:</a> All customers can get a parking ticket and pay for it.</li>
    <li>Parking Attendant: Parking attendants can do all the activities on the customer’s behalf, and can take cash for ticket payment.</li>
    <li>System: To display messages on different info panels, as well as assigning and removing a vehicle from a parking spot.</li>
  </ul>
  <ul>
    <li>Here are the top use cases for Parking Lot:</li>
    <li>Add/Remove/Edit parking floor: To add, remove or modify a parking floor from the system. Each floor can have its own display board to show free parking spots.</li>
    <li>Add/Remove/Edit parking spot: To add, remove or modify a parking spot on a parking floor.</li>
    <li>Add/Remove a parking attendant: To add or remove a parking attendant from the system.</li>
    <li>Take ticket: To provide customers with a new parking ticket when entering the parking lot.</li>
    <li>Scan ticket: To scan a ticket to find out the total charge.</li>
    <li>Credit card payment: To pay the ticket fee with credit card.</li>
    <li>Cash payment: To pay the parking ticket through cash.</li>
    <li>Add/Modify parking rate: To allow admin to add or modify the hourly parking rate.</li>
  </ul>
</p>
<img src="./images/Use%20Case%20Diagram.png" alt="Use Case Diagram">
</div>
<div>
  <h2>Activity Diagram</h2>
  <p>Customer paying for parking ticket: Any customer can perform this activity.</p>
  <img src="./images/Activity%20Diagram.png" alt="Activity Diagram">
</div>
<div>
<h2 style="color: brown;">Class Diagram</h2>
  <p>
  <ul>
  <li>ParkingLot: The central part of the organization for which this software has been designed. It has attributes like ‘Name’ to distinguish it from any other parking lots and ‘Address’ to define its location.</li>
  <li>ParkingFloor: The parking lot will have many parking floors.</li>
  <li>ParkingSpot: Each parking floor will have many parking spots. Our system will support different parking spots 1) Handicapped, 2) Compact, 3) Large, 4) Motorcycle, and 5) Electric.</li>
  <li>Account: We will have two types of accounts in the system: one for an Admin, and the other for a parking attendant.</li>
  <li>Parking ticket: This class will encapsulate a parking ticket. Customers will take a ticket when they enter the parking lot.</li>
  <li>Vehicle: Vehicles will be parked in the parking spots. Our system will support different types of vehicles 1) Car, 2) Truck, 3) Electric, 4) Van and 5) Motorcycle.</li>
  <li>EntrancePanel and ExitPanel: EntrancePanel will print tickets, and ExitPanel will facilitate payment of the ticket fee.</li>
  <li>Payment: This class will be responsible for making payments. The system will support credit card and cash transactions.</li>
  <li>ParkingRate: This class will keep track of the hourly parking rates. It will specify a dollar amount for each hour. For example, for a two hour parking ticket, this class will define the cost for the first and the second hour.</li>
  <li>ParkingDisplayBoard: Each parking floor will have a display board to show available parking spots for each spot type. This class will be responsible for displaying the latest availability of free parking spots to the customers.</li>
  <li>ParkingAttendantPortal: This class will encapsulate all the operations that an attendant can perform, like scanning tickets and processing payments.</li>
  <li>CustomerInfoPortal: This class will encapsulate the info portal that customers use to pay for the parking ticket. Once paid, the info portal will update the ticket to keep track of the payment.</li>
  <li>ElectricPanel: Customers will use the electric panels to pay and charge their electric vehicles.</li>
</ul>
<img src="./images/Class%20Diagram.png" alt="Class Diagram">
  </p>
</div>
