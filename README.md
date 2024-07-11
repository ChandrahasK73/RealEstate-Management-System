# RealEstate-Management-System
A Java Servlets based web application designed for Real-Estate-Management
# Real Estate Management Application

## Project Overview
The Real Estate Management application is designed to streamline various aspects of real estate operations. It allows users to register, add payment information, search for properties, and book properties. The application supports both agents and prospective renters, with features tailored to their specific needs.

## Key Features and Requirements

### 1. User Management
- **Registration**: Both agents and prospective renters can create an account using their email address.
- **Profile Management**: Users can update their personal details, payment methods, and addresses.

### 2. Property Management
- **Property Listings**: Agents can add, modify, and delete property listings. Each property includes attributes such as type, location, description, price, and availability.
- **Property Types**: The system handles various property types, including houses, apartments, commercial buildings, and additional types like vacation homes and land.

### 3. Search and Booking
- **Search Functionality**: Users can search for properties based on location, date, number of bedrooms, price range, and property type. Results can be sorted by price or number of bedrooms.
- **Booking**: Prospective renters can book properties, selecting the rental period and payment method. The application displays the booking details and calculates the total cost.

### 4. Payment and Address Management
- **Payment Methods**: Renters can manage their credit card information, associating each card with a billing address.
- **Address Management**: Users can add, modify, and delete addresses, ensuring that addresses linked to payment methods are not deleted prematurely.

### 5. Booking Management
- **Viewing and Managing Bookings**: Renters can view their bookings, check details, and cancel bookings if needed. Agents can view all bookings for their properties and also cancel bookings.

### Bonus Features
- **Neighborhood Information**: Additional information about neighborhoods, such as crime rates and nearby schools, can be included in the property listings.
- **Reward Program**: A reward program where renters earn points based on their bookings. Points can be accumulated and viewed by the renters.

## Data Requirements

### Entities and Attributes
1. **User**: 
   - `UserID`
   - `Name`
   - `Email`
   - `Phone`
   - `Address`
2. **Agent**: 
   - `AgentID`
   - `JobTitle`
   - `Agency`
   - `ContactInfo` (inherits from User)
3. **Perspective Renter**: 
   - `RenterID`
   - `Preferences`
   - `CreditCardInfo`
   - `PreferredLocation` (inherits from User)
4. **Property**: 
   - `PropertyID`
   - `Type`
   - `Location`
   - `Description`
   - `City`
   - `State`
   - `NumberOfRooms`
   - `SquareFootage`
   - `BuildingType`
   - `Price`
   - `Availability`
5. **Booking**: 
   - `BookingID`
   - `PropertyID`
   - `RenterID`
   - `CreditCardUsed`
   - `RentalPeriod`
   - `TotalCost`
6. **Credit Card**: 
   - `CardID`
   - `CardNumber`
   - `ExpirationDate`
   - `PaymentAddress`
7. **Address**: 
   - `AddressID`
   - `UserID`
   - `Street`
   - `City`
   - `State`
   - `ZipCode`
8. **PropertyType**: 
   - `TypeID`
   - `TypeName`
9. **Neighborhood**: 
   - `NeighborhoodID`
   - `CrimeRate`
   - `NearbySchools`
10. **AdditionalPropertyType**: 
    - `AdditionalTypeID`
    - `TypeName`
11. **RewardProgram**: 
    - `ProgramID`
    - `Points`

## ER Model
The ER model for this project includes entities such as User, Property, Booking, Credit Card, Address, PropertyType, Neighborhood, AdditionalPropertyType, and RewardProgram. The relationships between these entities are defined to manage the data efficiently and ensure that all user interactions and property transactions are handled smoothly.

## Project Structure
- **User Management**: Handling user registration and profile updates.
- **Property Management**: Allowing agents to manage property listings.
- **Search and Booking**: Enabling renters to search for and book properties.
- **Payment and Address Management**: Managing user payment methods and addresses.
- **Booking Management**: Viewing and managing bookings.
- **Bonus Features**: Incorporating neighborhood information and a reward program.

## Conclusion
This project aims to create a robust real estate management system that provides a seamless experience for both agents managing properties and renters looking for their next home.
