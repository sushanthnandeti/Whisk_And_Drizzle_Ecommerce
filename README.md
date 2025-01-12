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

1. **Scheduling with Amazon EventBridge**  
2. **AWS Lambda Execution**  
3. **Email Delivery via Amazon SES**  
4. **Monitoring and Logs**  

This end-to-end setup ensures timely and automated email distribution to users with minimal manual intervention—both **scalable** and **cost-efficient**.

## YouTube
For a quick walkthrough of **Whisk and Drizzle**, check out our demo video on YouTube:  
[Whisk and Drizzle Demo](https://www.youtube.com/watch?v=lrMMvK9tjGw)
