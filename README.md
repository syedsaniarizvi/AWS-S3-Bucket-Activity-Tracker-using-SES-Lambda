# AWS-S3-Bucket-Activity-Tracker-using-SES-Lambda


**Introduction**

In the realm of cloud computing, Amazon Web Services (AWS) offers a comprehensive suite of services for scalable and reliable infrastructure management. Among these services, Amazon Simple Storage Service (S3) stands out as a key component for storing and retrieving data over the internet. Monitoring activities within S3 buckets, such as object creation and deletion, is crucial for maintaining data integrity and security. To address this need, the AWS S3 Bucket Activity Tracker project provides a solution to track and notify users about such activities.

**Abstract**

The AWS S3 Bucket Activity Tracker is a serverless project aimed at monitoring and tracking activities within AWS S3 buckets. Leveraging services such as Amazon Simple Email Service (SES), Identity and Access Management (IAM), Amazon S3, and AWS Lambda, this project automates the process of sending email notifications containing information about S3 bucket activities. By utilizing serverless architecture, the project ensures scalability, cost-effectiveness, and minimal maintenance overhead.

**Services Used**

Amazon SES (Simple Email Service): Used for sending email notifications to users, providing a reliable and scalable email delivery solution.
IAM (Identity and Access Management): Manages access permissions and security policies for AWS resources, ensuring secure interactions between services.
Amazon S3: Serves as the primary storage for tracking activity logs and storing objects. It is also the focal point of monitoring for bucket activity.
AWS Lambda: Executes serverless functions triggered by S3 bucket events, enabling seamless automation of activity tracking and notification generation.
Procedure (Step-wise Implementation)
Set Up IAM Roles: Create IAM roles with appropriate permissions to allow Lambda functions to interact with S3 buckets and SES for sending emails.
Configure S3 Event Notifications: Configure S3 bucket event notifications to trigger AWS Lambda functions upon object creation or deletion.
Develop Lambda Functions: Write Lambda functions to process S3 events, extract relevant information (such as bucket names and object names), and trigger email notifications using SES.
Set Up SES Configuration: Configure SES to send emails, including defining sender and recipient addresses and verifying domain identities.
Deploy Lambda Functions: Deploy Lambda functions to the AWS Lambda service.
Test Configuration: Test the setup by creating or deleting objects within the monitored S3 buckets and verifying that email notifications are received.

**Applications and Use Cases**

Data Governance: Monitor changes in S3 buckets to ensure compliance with data governance policies.
Security Monitoring: Detect unauthorized access or data breaches by tracking S3 activity.
Operational Insights: Gain insights into usage patterns and trends by analyzing S3 activity logs.
Compliance Reporting: Generate reports on S3 activity for compliance audits and regulatory requirements.

**Conclusion**
The AWS S3 Bucket Activity Tracker project provides a robust solution for monitoring and tracking activities within S3 buckets, enhancing visibility and control over data storage environments. By leveraging serverless architecture and AWS services such as Lambda, S3, SES, and IAM, the project offers a scalable, cost-effective, and automated approach to S3 activity tracking. With its ease of implementation and broad applicability, this project serves as a valuable tool for AWS users seeking to enhance their data management practices and maintain compliance with security and governance standards.
