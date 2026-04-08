M-Pesa Daraja API Integration (Spring Boot)

📌 Overview

This project is a simple backend application that shows how to integrate M-Pesa payments using the Safaricom Daraja API with Spring Boot. It covers the basics of handling Customer-to-Business (C2B) transactions as well as initiating STK Push requests.

The main goal was to understand how M-Pesa APIs work and how they can be connected to a real backend system.

---

🚀 Features

- Generate and use OAuth access tokens from Daraja API
- Simulate C2B payments in the sandbox environment
- Initiate STK Push requests to a mobile number
- Handle callback responses from M-Pesa
- Expose simple REST endpoints for testing

---

🛠️ Tech Stack

- Java
- Spring Boot
- Gradle
- M-Pesa Daraja API

---

⚙️ Setup Instructions

1. Clone the repository

git clone https://github.com/YOUR_USERNAME/YOUR_REPO.git

2. Add your credentials

Open "application.properties" and update:

mpesa.consumerKey=YOUR_CONSUMER_KEY
mpesa.consumerSecret=YOUR_CONSUMER_SECRET
mpesa.shortCode=YOUR_SHORT_CODE

3. Run the application

You can run the project using your IDE or:

./gradlew bootRun

---

📡 API Endpoints

- GET /mpesa/token
  Generates an access token

- POST /mpesa/stk
  Sends an STK Push request

- POST /mpesa/callback
  Receives M-Pesa transaction response

---

📱 Testing

You can test the endpoints using Postman or any API testing tool.

Make sure phone numbers are in this format:

2547xxxxxxx

---

⚠️ Notes

- This project uses the Daraja sandbox (test environment)
- Do not share or commit your API credentials
- Replace all placeholder values before running

---

👥 Contributors

- Ian Bryan
- joeahkim

---

📄 License

This project is for learning purposes.

---

📈 Future Improvements

- Add a database to store transactions
- Improve error handling and logging
- Add authentication/security
- Deploy the app to a cloud platform

---

🙌 Acknowledgements

Thanks to Safaricom for providing access to the Daraja API for developers.
