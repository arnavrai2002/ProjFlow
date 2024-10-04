# ProjFlow

**ProjFlow** is a comprehensive project management tool designed to streamline project workflows, powered by a modern technology stack including Next.js, Node.js, Prisma ORM, PostgreSQL, and AWS cloud services.

---

## 𝐓𝐞𝐜𝐡𝐧𝐨𝐥𝐨𝐠𝐲 𝐒𝐭𝐚𝐜𝐤

### 𝐅𝐫𝐨𝐧𝐭𝐞𝐧𝐝
- **Framework**: Next.js
- **Styling**: Tailwind CSS
- **State Management**: Redux Toolkit, Redux Toolkit Query
- **UI Components**: Material UI Data Grid


### 𝐁𝐚𝐜𝐤𝐞𝐧𝐝
- **Framework**: Node.js with Express
- **ORM**: Prisma (PostgreSQL ORM)
- **Database**: PostgreSQL, managed with PgAdmin


### 𝐂𝐥𝐨𝐮𝐝 𝐒𝐞𝐫𝐯𝐢𝐜𝐞𝐬
- **AWS EC2**: Hosting the server
- **AWS RDS**: Managing PostgreSQL database
- **AWS API Gateway**: Handling API traffic
- **AWS Amplify**: Frontend hosting and deployment
- **AWS S3**: Storing static assets
- **AWS Lambda**: Serverless computing for various tasks
- **AWS Cognito**: Authentication service
- **Amazon CloudWatch**: Monitoring and logs
- **Amazon SNS**: Notifications
- **AWS Key Management Service (KMS)**: Managing encryption keys
- **AWS Data Transfer**: Managing data movement


---

## 𝐏𝐫𝐞𝐫𝐞𝐪𝐮𝐢𝐬𝐢𝐭𝐞𝐬

Ensure you have the following tools installed:

- [Git](https://git-scm.com/)
- [Node.js](https://nodejs.org/en/)
- [npm](https://www.npmjs.com/) (Node Package Manager)
- [PostgreSQL](https://www.postgresql.org/download/)
- [PgAdmin](https://www.pgadmin.org/download/)

---

## 𝐈𝐧𝐬𝐭𝐚𝐥𝐥𝐚𝐭𝐢𝐨𝐧 𝐒𝐭𝐞𝐩𝐬

1. **Clone the repository:**
   ```bash
   git clone [git url] ProjFlow

2. **Install dependencies:**

For the client:

bash

cd client
npm install

For the server:

bash

cd ../server
npm install

Set up the database:

bash

npx prisma generate
npx prisma migrate dev --name init
npm run seed

Configure environment variables:

    .env for server settings:
        PORT
        DATABASE_URL
    .env.local for client settings:
        NEXT_PUBLIC_API_BASE_URL

Run the project:

bash

    npm run dev

𝐀𝐖𝐒 𝐀𝐜𝐜𝐨𝐮𝐧𝐭 𝐒𝐞𝐭𝐮𝐩

    AWS IAM User
        Set up an IAM user with necessary permissions.
        Create access keys for programmatic access to AWS services.
        Assign roles based on least privilege.

    AWS Key Management Service (KMS)
        Use KMS to manage encryption keys for securing sensitive data.
        Apply key management to critical AWS services.

    AWS RDS
        Launch an RDS instance (PostgreSQL) for data management.
        Configure security groups to limit access to authorized services.

    Amazon Cognito
        Set up Cognito for user authentication.
        Manage signup, login, and social login (Google, Facebook).

    Amazon API Gateway
        Create RESTful APIs using API Gateway.
        Set up routes and methods for backend services.

    Amazon SNS
        Set up SNS for real-time notifications.
        Create an SNS topic and subscribe services to receive alerts.

    Amazon CloudWatch
        Monitor logs and metrics with CloudWatch.
        Set up alarms for API and Lambda monitoring.

    AWS Lambda
        Implement serverless functions using AWS Lambda for dynamic tasks.

    Amazon EC2
        Launch an EC2 instance to host the backend services.
        Configure security groups and set up key pairs.

    Amazon S3
        Create S3 buckets for static file storage and backups.
        Set up lifecycle rules for file versioning and automatic management.

    AWS Amplify
        Deploy and host the frontend via AWS Amplify.
        Enable continuous deployment (CI/CD) by connecting the repository.
