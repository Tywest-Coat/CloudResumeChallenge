# Cloud Resume Challenge - AWS

This repository contains the implementation details of the **Cloud Resume Challenge** for AWS. Below is an outline of the steps I completed, along with the technologies and tools used for each stage.

---

## **Overview of Completed Steps**

### **1. Certification**
I achieved the **AWS Certified Cloud Practitioner** certification, demonstrating my foundational knowledge of the AWS ecosystem. This certification is showcased on my resume.

### **2. HTML**
I built my resume in **HTML**, ensuring it is web-friendly and accessible. The raw structure of the content was written in semantic HTML for better readability and maintainability.

### **3. CSS**
To enhance the visual appearance of my resume, I styled it using **CSS**. While not overly complex, the design is clean, responsive, and user-friendly.

### **4. Static Website**
The HTML and CSS files were deployed to an **Amazon S3** bucket configured to host a static website. This ensures high availability and durability for my resume.

### **5. HTTPS**
I secured the website by integrating **Amazon CloudFront** with the S3 bucket to serve content over HTTPS. This improves security and ensures encrypted communication.

### **6. DNS**
I registered a custom domain and pointed it to the CloudFront distribution using **Amazon Route 53**. My resume is now accessible at [resume.tylerwestcoat.com](http://resume.tylerwestcoat.com).

### **7. JavaScript**
I added a **visitor counter** to my resume page using **JavaScript**, which dynamically fetches and displays the number of visits.

### **8. Database**
The visitor count is stored in an **Amazon DynamoDB** table. This NoSQL database ensures scalability and low-cost storage.

### **9. API**
I created a **REST API** using **AWS API Gateway** and **AWS Lambda**. This API serves as the bridge between the JavaScript front end and the DynamoDB database.

### **10. Python**
The logic for the API was written in **Python**, leveraging the **boto3** library to interact with DynamoDB. This modular and efficient code updates and retrieves the visitor count.

### **11. Tests**
I wrote unit tests for the Python code using the **unittest** framework. These tests ensure the reliability and correctness of the Lambda function logic.

### **12. Infrastructure as Code (IaC)**
I defined all back-end resources (API Gateway, Lambda, DynamoDB) using the **AWS Serverless Application Model (SAM)** template. This approach provides reproducibility and automation for infrastructure setup.

### **13. Source Control**
I created two **GitHub repositories**:
- **Frontend Repository**: Contains the HTML, CSS, and JavaScript files for the resume.
- **Backend Repository**: Contains the SAM template and Python code for the API.

### **14. CI/CD (Back end)**
I implemented a **CI/CD pipeline** for the backend using **GitHub Actions**:
- The pipeline runs tests automatically when code is pushed.
- If tests pass, the SAM application is packaged and deployed to AWS.

### **15. CI/CD (Front end)**
I implemented a **CI/CD pipeline** for the frontend using **GitHub Actions**:
- Any updates to the frontend code automatically upload to the S3 bucket.
- The pipeline also invalidates the CloudFront cache to ensure updated content is served.

---

## **Technologies Used**
- **AWS Services**: S3, CloudFront, Route 53, DynamoDB, API Gateway, Lambda
- **Programming Languages**: HTML, CSS, JavaScript, Python
- **Frameworks/Tools**: AWS SAM, GitHub Actions
- **Testing Frameworks**: unittest (Python)
- **Source Control**: GitHub

---

## **How to Access**
Visit my resume at [resume.tylerwestcoat.com](http://resume.tylerwestcoat.com).

---

Feel free to explore the repositories and provide feedback!
