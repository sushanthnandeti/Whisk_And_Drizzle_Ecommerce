# Whisk and Drizzle — Application Overview

**Whisk and Drizzle** is a full-stack E-Commerce platform specializing in desserts. It integrates with Stripe for secure payment processing and includes a coupon system to allow customers to apply discounts at checkout. The frontend is built with ReactJS and uses Zustand for global state management, while the backend is powered by Node.js and Express.

To ensure continuous delivery and rapid iteration, Whisk and Drizzle is deployed via a **Jenkins CI/CD pipeline**, with an **NGINX** server handling routing and static file serving. The entire infrastructure is hosted on **AWS**, providing a scalable environment for growing business needs.

## Key Highlights

- **Stripe Payment Gateway**  
- **Coupon/Discount System**  
- **React + Zustand Frontend**  
- **Node.js + Express Backend**  
- **Jenkins CI/CD**  
- **NGINX Servers**  
- **AWS Infrastructure**  

## Automated Email System

# Automated System Overview

![Automated AWS System](https://whiskanddrizzle.s3.us-east-1.amazonaws.com/email.png)

This system automates email sending to users by leveraging **Amazon EventBridge**, **AWS Lambda**, and **Amazon Simple Email Service (SES)**. Here’s how it works:

This system automates email sending to users by leveraging **Amazon EventBridge**, **AWS Lambda**, and **Amazon Simple Email Service (SES)**. Here’s how it works:

1. **Scheduling with Amazon EventBridge**  
   - A rule is configured in EventBridge to trigger at specific intervals (e.g., daily, weekly).
   - When the trigger fires, it invokes the AWS Lambda function.

2. **AWS Lambda Execution**  
   - The Lambda function contains the core logic for preparing and sending emails.
   - It can read or store relevant data in **Amazon Simple Storage Service (S3)** if needed (e.g., retrieving templates or user data, or writing logs).

3. **Email Delivery via Amazon SES**  
   - Once the Lambda function gathers the necessary information, it uses Amazon SES to send out emails to the designated users.
   - SES handles the email infrastructure, ensuring deliverability and tracking (bounce, complaints, etc.).

4. **Monitoring and Logs**  
   - You can view logs and execution metrics (e.g., function duration, invocations) from AWS CloudWatch to monitor performance and troubleshoot if needed.

In the screenshot above:
- **Left**: You can see the `EmailToUsers` schedule details configured in EventBridge.  
- **Center**: A snippet of the Lambda function’s Node.js code.  
- **Right**: A code editor view for the Lambda function, showing how the payload and logic are structured.
This end-to-end setup ensures timely and automated email distribution to users with minimal manual intervention—both **scalable** and **cost-efficient**.

## YouTube
For a quick walkthrough of **Whisk and Drizzle**, check out our demo video on YouTube:  
[Whisk and Drizzle Demo](https://www.youtube.com/watch?v=lrMMvK9tjGw)
