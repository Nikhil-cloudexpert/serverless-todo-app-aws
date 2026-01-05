# Serverless To-Do List Application (AWS)

A serverless personal To-Do List application built using AWS services.  
The project demonstrates how to build a scalable, cost-effective backend using AWS Lambda, API Gateway, and DynamoDB without managing servers.

---

## 🚀 Architecture Overview

Client → API Gateway → AWS Lambda → DynamoDB

The application follows an event-driven, serverless architecture where each HTTP request triggers a Lambda function that performs CRUD operations on DynamoDB.

---

## 🛠 AWS Services Used

- **AWS Lambda** – Backend logic for CRUD operations  
- **Amazon API Gateway** – REST API endpoints  
- **Amazon DynamoDB** – NoSQL database for task storage  
- **AWS IAM** – Secure access between services  
- **Amazon CloudWatch** – Logs and monitoring  

---

## 📌 Features

- Create a task  
- Retrieve all tasks  
- Update an existing task  
- Delete a task  
- Fully serverless (no EC2 / no servers)

---

## 🔗 API Endpoints

| Method | Endpoint | Description |
|------|--------|------------|
| POST | `/todo` | Create a new task |
| GET | `/todo` | Get all tasks |
| PUT | `/todo` | Update a task |
| DELETE | `/todo?id=1` | Delete task by ID |

---

## 🧪 Sample API Events

Sample API Gateway events are available in the `sample-events/` folder to simulate requests locally or understand event structure.

---

## 🧱 Lambda Logic

A single Lambda function handles all CRUD operations by routing logic based on HTTP method:
- POST → Create task
- GET → Read tasks
- PUT → Update task
- DELETE → Delete task

Code is available in `lambda/todoHandler.js`.

---

## 📄 Documentation

A detailed project report explaining architecture, workflow, and implementation is available in the `docs/` folder.

---

## 🎯 Learning Outcomes

- Understanding serverless architecture  
- Hands-on experience with AWS Lambda, API Gateway, DynamoDB  
- Designing RESTful APIs  
- Working with event-driven cloud systems  

---

## 👤 Author

**Nikhil Singh**
