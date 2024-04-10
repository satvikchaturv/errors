# Examination Smart Contract

## Overview
This Solidity smart contract, named `Examination`, is designed to manage examination-related data and criteria for students or participants. It includes functionalities to update attendance, as well as exam attempt criteria such as the number of attempts allowed and minimum age requirement.

## Functionality

### `constructor()`
- Initializes the contract by setting default values for `attendance`, `attemptNumber`, and `age` to zero.

### `updateAttendance(uint256 _attendance)`
- Allows updating the attendance percentage for a participant.
- Requires the attendance percentage to be greater than or equal to 75%.
- Parameters:
  - `_attendance`: The new attendance percentage to be set.

### `updateExamCriteria(uint256 _attemptNumber, uint256 _age)`
- Allows updating the exam attempt criteria, including the number of attempts allowed and the minimum age requirement.
- Checks if the age is greater than or equal to 18 years.
- If the number of attempts exceeds 3, it reverts with an error message indicating no attempts are left to write the exam.
- Parameters:
  - `_attemptNumber`: The new attempt number allowed for the exam.
  - `_age`: The new minimum age requirement for the exam.

## Smart Contract Usage
- Deploy the smart contract onto a compatible blockchain network.
- Interact with the contract using Ethereum-compatible wallets or dApps to update attendance and exam criteria.

## License
This smart contract is licensed under the MIT License, as indicated by the SPDX-License-Identifier in the contract code.
