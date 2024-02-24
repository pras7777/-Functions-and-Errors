# Functions-and-Errors


### Overview
This Solidity smart contract, named `StudentDatabase`, serves as a simple database for storing student profiles. It implements various functions for creating, updating, deleting, and viewing student profiles. The contract also demonstrates the use of `require()`, `assert()`, and custom errors for error handling.

### Smart Contract Structure
- **Student Struct**: Defines the structure of a student, including attributes like name, age, and technical stack.
- **Mapping**: Utilizes a mapping to associate each Ethereum address with a corresponding student profile.
- **Functions**:
  - `createStudentProfile`: Allows users to create a new student profile.
  - `confirmStudentName`: Verifies if the provided name matches the name associated with the caller's address.
  - `confirmStudentAge`: Verifies if the provided age matches the age associated with the caller's address.
  - `confirmStudentTechStack`: Verifies if the provided technical stack matches the stack associated with the caller's address.
  - `updateProfile`: Enables users to update their existing student profile.
  - `deleteProfile`: Allows users to delete their student profile.
  - `viewProfile`: Retrieves and returns the details of the caller's student profile.

### Error Handling
- **Custom Error**: `ProfileDoesNotExist` is a custom error thrown when attempting to access a profile that does not exist.
- **Requirements**:
  - The name provided during profile creation must be longer than 4 characters.
  - The age provided during profile creation cannot be zero.
  - The technical stack provided during profile creation must be longer than 4 characters.

### Usage
1. **Deployment**: Deploy the `StudentDatabase` contract to the Ethereum blockchain.
2. **Interacting with the Contract**: Users can interact with the contract through various functions to manage student profiles:
   - Create a new profile.
   - Confirm profile details.
   - Update existing profile.
   - Delete profile.
   - View profile details.

### Testing
- Ensure to test all functionalities thoroughly before deploying the contract in a production environment.
- Test different scenarios, including valid and invalid inputs, to ensure proper functionality and error handling.

### License
This smart contract is licensed under the MIT License.
