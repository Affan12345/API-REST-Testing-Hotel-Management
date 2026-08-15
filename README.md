## 🏨 RESTful Booker API Automation Project

## 📌 Project Overview

This project demonstrates automated end-to-end API testing using **Postman** and **Newman CLI** for the RESTful Booker service. It covers the complete testing workflow, including creating, updating, retrieving, dynamic data generation, and deleting booking information through REST APIs.

The project also includes automated test assertions, authentication token management, environment variable mapping, dynamic payload generation, and interactive HTML execution report generation using Newman.

---

## 🛠️ Tools & Technologies

- Postman
- Newman CLI
- HTMLExtra Reporter
- Git & GitHub
- REST API
- JSON Data Validation
- JavaScript (Pre-request & Test Scripts)

  
## 📁 Project Structure

```text
API-REST-Testing-Hotel-Management
│
│├── Postman_Collection
│   └── API_Testing.postman_collection.json
│
├── Environment
│   └── EnvironmentAPITesting.postman_environment.json
│
├── Automation_Report
│   └── API_Testing_Report.html
│
└── README.md


```
# 🧪 Test Scenarios & Workflows

1. Get Bookings ID (GET /booking)
   • Retrieves all existing booking IDs.
   • Validates response HTTP status code (200 OK) and latency response time.

2. Create Booking (POST /booking)
   • Dynamically generates test data (random names, prices, dates).
   • Saves the returned bookingid into the environment variable.

3. Get Specific Booking ID (GET /booking/:id)
   • Fetches details of the newly created booking ID.
   • Validates response payload structure and field values.

4. Create Auth Token (POST /auth)
   • Sends admin credentials (admin / password123).
   • Captures and stores access token into environment variables.

5. Update Booking (PATCH /booking/:id)
   • Authenticates using the generated token.
   • Updates target booking details.

6. Delete Booking (DELETE /booking/:id)
   • Removes target booking from the system.
   • Verifies HTTP status code for deletion.

## 📁Verifies HTTP status code for deletion confirmation.

How to Run the Project
##Prerequisites

Make sure you have Node.js installed.

Step 1: Install Dependencies

npm install -g newman newman-reporter-htmlextra

Step 2: Run Collection via Newman CLI

newman run Postman_Collection/API_Testing.postman_collection.json -e Environment/EnvironmentAPITesting.postman_environment.json -r cli,htmlextra --reporter-htmlextra-export ./Automation_Report/API_Testing_Report.html

## 📁Execution Report
After running the tests, an interactive dashboard report will be generated inside the Automation_Report/ directory. Open API_Testing_Report.html in any browser to inspect:

Overall execution summary (Passed/Failed test counts)

Response times and payload sizes

Detailed assertion logs and HTTP headers

Attach the Report file to the repository

---

## 🤝 Contributing & Feedback

Contributions, issues, and feature requests are welcome! If you have any suggestions or find any bugs, feel free to open an issue or submit a pull request.

---

## 📜 License

This project is open-source and available under the **[MIT License](LICENSE)**.

---

## 🧑‍💻 Author

**Affan**
* GitHub: [@Affan12345](https://github.com/Affan12345)
* Project Repo: [API-REST-Testing-Hotel-Management](https://github.com/Affan12345/API-REST-Testing-Hotel-Management)

---

<p align="center">
  <b>⭐ If you found this project helpful, don't forget to give it a star on GitHub! ⭐</b>
</p>

