# KitSoft - Full-Stack Application with Next.js, Vercel Auth, and Vercel Database

KitSoft is a modern full-stack web application built with **Next.js**, **Vercel Authentication**, and **Vercel Database** for managing tasks, tracking performance, and real-time collaboration.

## Features
- **User Authentication** with Vercel Authentication.
- **Real-time Database** powered by **Vercel Database**.
- **Responsive UI** built with Tailwind CSS.
- **Deployed on Vercel** for fast and reliable performance.

---

## Getting Started

### Prerequisites
Make sure you have the following installed:
- [Node.js](https://nodejs.org/) (v16 or later)
- [Vercel CLI](https://vercel.com/cli) (optional for deployment)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/KitSoft.git
   cd KitSoft
   ```
2. **Install dependencies**
   ```bash
   npm install
   ```
3. **Set up environment variables**
  Create a .env file in the root directory and add the following:
   ```bash
   NEXTAUTH_URL=http://localhost:3000
   NEXTAUTH_SECRET=your-secret-key
   DATABASE_URL=vercel-database-url
   ```
   Note: Replace your-secret-key with a secure key and vercel-database-url with your Vercel Database connection string.

4. **Start the development server**
   ```bash
   npm run dev
   ```
Open http://localhost:3000 in your browser to see the app.


###Tech Stack
	•	Framework: Next.js
	•	Authentication: Vercel Authentication
	•	Database: Vercel Database
	•	Deployment: Vercel
	•	UI: Tailwind CSS

 ###Deployment on Vercel
	1.	Push your code to a GitHub repository.
	2.	Connect the repository to your Vercel account.
	3.	Set environment variables in the Vercel dashboard.
	4.	Deploy the project with a single click.

 ###Database Setup (Vercel Database)
 	1.	Go to your Vercel dashboard and create a new Vercel Database.
	2.	Set up your schema and tables.
	3.	Add your DATABASE_URL to your environment variables in Vercel.
	4.	Use the Vercel Database client in your app for querying and managing data.

Example query with Vercel Database:
```javascript
import { db } from '@vercel/database';

const getData = async () => {
  const result = await db.query('SELECT * FROM tasks');
  return result.rows;
};
```

