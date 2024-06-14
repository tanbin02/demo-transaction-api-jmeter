# Performance Testing with Apache JMeter

This project involves automating a series of positive test cases using Apache JMeter. The objective is to simulate the actions of an admin, agent, and customer in a financial transaction system, and measure the performance of the system under test.

## Test Scenario

The test scenario includes the following steps:

1. **Admin creates an agent and a customer.**
2. **Deposit 2000 TK to the agent from the system account.**
3. **Deposit 1000 TK to the customer from the agent account.**
4. **Check balance from the customer account.**
5. **Withdraw 500 TK from the customer account.**
6. **Payment of 200 TK from the customer account to a merchant.**

## Requirements

- Apache JMeter installed on your machine
- Basic understanding of JMeter and performance testing
- A working instance of the financial transaction system to test against

## Setup Instructions

1. **Install Apache JMeter:**
   - Download and install Apache JMeter from the [official website](https://jmeter.apache.org/download_jmeter.cgi).

2. **Clone the Repository:**
   - Clone or download the project repository containing the JMX file.

3. **Open the JMX file:**
   - Launch JMeter and open the provided `.jmx` file.

## Creating the Test Plan

1. **Add a Thread Group:**
   - Set the number of threads (users), ramp-up period, and loop count.

2. **Add HTTP Requests:**
   - **Create Agent and Customer:**
     - Add an HTTP Request sampler to create an agent.
     - Add another HTTP Request sampler to create a customer.
   - **Deposit to Agent:**
     - Add an HTTP Request sampler to deposit 2000 TK to the agent from the system account.
   - **Deposit to Customer:**
     - Add an HTTP Request sampler to deposit 1000 TK to the customer from the agent account.
   - **Check Customer Balance:**
     - Add an HTTP Request sampler to check the customer's account balance.
   - **Withdraw from Customer:**
     - Add an HTTP Request sampler to withdraw 500 TK from the customer's account.
   - **Payment to Merchant:**
     - Add an HTTP Request sampler to make a payment of 200 TK from the customer's account to a merchant.

3. **Add Listeners:**
   - Include listeners such as View Results Tree, Summary Report, and Aggregate Report to monitor and analyze the test results.

## Running the Test

1. **Configure HTTP Request Defaults:**
   - Set the server name or IP, port number, and other default parameters for HTTP requests.

2. **Start the Test:**
   - Run the test plan by clicking the green start button in JMeter.

3. **Analyze Results:**
   - Use the listeners to analyze the performance and response of the system under test

## Output:
## jmeter html report:
![image](https://github.com/tanbin02/demo-transaction-api-jmeter/assets/95366983/a573943d-3559-4351-89f8-66b8ca7cad59)


## Conclusion

By following these steps, you can create a JMX file in Apache JMeter to automate and measure the performance of a financial transaction system. This setup will help ensure the system can handle various operations efficiently and provide insights into potential performance bottlenecks.


