# Medical Information System

A C++ program for managing patient records in a medical facility.The data is stored in a structured format using arrays, ensuring easy access and management of patient information.

## Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Functions](#functions)
- [Data Storage](#data-storage)
- [File Handling](#file-handling)
- [Contributing](#contributing)
- 
## Features

- **Add Patient Record**: Enter and store patient details including name, CNIC, gender, disease, past medical history, and check-in date.
- **Delete Patient Record**: Remove patient records using a unique registration ID.
- **Display All Records**: View all stored patient records.
- **Search Patient Record**: Search for a patient using their registration ID.
- **Save Records**: Save current patient records to a file.
- **Retrieve Records**: Retrieve patient records from a file.

## Getting Started

### Prerequisites

- A C++ compiler supporting C++11 or later.
- C++ Standard Library.

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/medical-information-system.git
    ```

2. Navigate to the project directory:
    ```bash
    cd medical-information-system
    ```

3. Compile the program:
    ```bash
    g++ -std=c++11 main.cpp -o medical_info_system
    ```

4. Run the program:
    ```bash
    ./medical_info_system
    ```

## Usage

Follow the on-screen prompts to navigate through the menu and manage patient records. The program allows you to add, delete, display, search, save, and retrieve patient records.

## Functions

### `bool validateCnic(const string& cnic)`

Validates the CNIC format to ensure it matches the pattern `xxxxx-xxxxxxx-x`.

### `string getCurrentDate()`

Returns the current date in `YYYY-MM-DD` format.

### `void ADDrecord(string Names[], string Regids[], string Cnics[], string Genders[], string Dates[], string Pastmedicalhistory[], string Diseases[], const string& firstName, const string& middleName, const string& lastName, const string& cnic, const string& gender, const string& date, const string& pasthistory, const string& regid, const string& disease, int& patientcount, int maxcapacity)`

Adds a new patient record to the system.

### `void Delrecord(string Names[], string Regids[], string Cnics[], string Genders[], string Dates[], string Pastmedicalhistory[], string Diseases[], const string& regid, int& patientcount)`

Deletes a patient record based on the registration ID.

### `void Patientdisplay(string Names[], string Regids[], string Cnics[], string Genders[], string Dates[], string Pastmedicalhistory[], string Diseases[], int& patientcount)`

Displays all patient records.

### `void Searchpatient(string Names[], string Regids[], string Cnics[], string Genders[], string Dates[], string Pastmedicalhistory[], string Diseases[], const string& regid, int& patientcount)`

Searches for a patient record using the registration ID.

### `void Saverecord(string Names[], string Regids[], string Cnics[], string Genders[], string Dates[], string Pastmedicalhistory[], string Diseases[], const string& filename, int patientcount)`

Saves all current patient records to a file.

### `void retriveRecord(const string& filename)`

Retrieves and displays patient records from a file.

## Data Storage

- **Arrays**: The program uses arrays to store patient details including names, registration IDs, CNICs, genders, dates, past medical histories, and diseases.

## File Handling

- Records are saved to and retrieved from a file named `record.txt`.
- Ensure you have the necessary file permissions to read/write to `record.txt`.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.
