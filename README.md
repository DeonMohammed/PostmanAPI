# Test Plan: Restful-Booker API

## Introduction

**Objective:** Validate the functionality and performance of the Restful-Booker API.
**Scope:** Functional testing of CRUD operations and API endpoints.
**Tools:** Postman for API testing and validation.

## Test Environment

- **Environment:** BookerEnv
- **Base URL:** `https://restful-booker.herokuapp.com`

## Test Strategy

- **Automation Tool:** Postman
- **Testing Types:** Functional, Performance

## Test Cases

Each test case covers different scenarios for the API endpoints specified in the collection.

### Test Case Table

| **Test Case ID** | **Endpoint**                        | **HTTP Method** | **Description**                                                                                           | **Expected Result**                                                                                      | **Notes**                                                                                                  |
|------------------|-------------------------------------|-----------------|-----------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------|
| TC001            | Health Check                        | GET             | Verify if the service is up and running.                                                                  | Response status code is 201. Response time is less than 1500ms.                                           |                                                                                                            |
| TC002            | Get All Booking IDs                 | GET             | Retrieve all booking IDs.                                                                                 | Response status code is 200. Response time is less than 1500ms.                                           |                                                                                                            |
| TC003            | Get Booking Details                 | GET             | Retrieve details of a specific booking (e.g., booking ID 1521).                                           | Response status code is 200. Response time is less than 1500ms.                                           |                                                                                                            |
| TC004            | Get All Booking by Name             | GET             | Retrieve bookings by first name 'John' and last name 'Smith'.                                              | Response status code is 200. Response time is less than 1500ms.                                           |                                                                                                            |
| TC005            | Get All Booking by Additional Needs | GET             | Retrieve bookings where additional needs include 'Breakfast'.                                              | Response status code is 200. Response time is less than 1500ms.                                           |                                                                                                            |
| TC006            | Get All Booking with Deposit Paid   | GET             | Retrieve bookings where deposit is marked as paid.                                                         | Response status code is 200. Response time is less than 1000ms.                                           | Ensure response time is optimized due to higher priority.                                                  |
| TC007            | Create Booking                      | POST            | Create a new booking with specific details.                                                                | Response status code is 200. Response time is less than 1500ms.                                           | Verify booking creation with exactness of booking details.                                                 |
| TC008            | Create Token                        | POST            | Authenticate with credentials to generate a token.                                                         | Response status code is 200. Response time is less than 1500ms.                                           | Check proper authentication process that does not take much time.                                          |
| TC009            | Update Booking                      | PUT             | Update booking details for booking ID 1521.                                                                | Response status code is 200. Response time is less than 1500ms.                                           | Ensure the same booking ID with its specific id is required.                                              |



This README provided an overview of the Restful-Booker API along with its test plan and test cases using Postman. For more details, refer to the [full documentation](#) or explore the [API collection](#) directly in Postman.

If you have any questions, feedback, or issues, please feel free to [contact us](#) or open an [issue](#) on GitHub.

Thank you for using Restful-Booker!

