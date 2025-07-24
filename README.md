# Threads - A Full-Stack Next.js Application

This is a full-stack, feature-rich social media application inspired by Threads. It's built with a modern tech stack centered around Next.js 14 and demonstrates a wide range of web development skills, from complex database schemas to real-time updates and third-party API integration.

![Threads Demo](https://i.imgur.com/Q21zZbY.png)

---

## Features

* **Complete User Authentication**: Secure sign-up and sign-in functionality using Clerk, including social providers like Google and GitHub.
* **Create & Manage Threads**: Users can create, comment on, and manage their own posts.
* **Nested Comments**: A multi-level comment system for engaging discussions.
* **Communities**: Users can create and join communities, post threads within them, and manage members.
* **Activity Feed**: A real-time notification system to track interactions.
* **User Profiles**: Customizable user profiles with threads, replies, and community information.
* **Advanced Search**: Robust search functionality to find other users and communities, complete with pagination.
* **File Uploads**: Seamless image uploads for profile pictures and thread content, powered by UploadThing.

---

## Tech Stack

* **Framework**: Next.js 14
* **Language**: TypeScript
* **Database**: MongoDB with Mongoose
* **Authentication**: Clerk
* **Styling**: Tailwind CSS & Shadcn UI
* **File Uploads**: UploadThing
* **Form Management**: React Hook Form
* **Validation**: Zod
* **Deployment**: Vercel

---

## Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

* Node.js (v18 or later)
* Git
* MongoDB Atlas account
* Clerk account
* UploadThing account

### Installation

1.  **Clone the repository:**
    ```sh
    git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git)
    ```
2.  **Navigate to the project directory:**
    ```sh
    cd YOUR_REPOSITORY
    ```
3.  **Install dependencies:**
    ```sh
    npm install
    ```
4.  **Set up your environment variables:**
    Create a file named `.env.local` in the root of the project and add the following, replacing the placeholder values with your actual credentials.
    ```
    # Clerk
    NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
    CLERK_SECRET_KEY=
    NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
    NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
    NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
    NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/onboarding

    # MongoDB
    MONGODB_URL=

    # UploadThing
    UPLOADTHING_SECRET=
    UPLOADTHING_APP_ID=

    # Webhook
    CLERK_WEBHOOK_SECRET=
    ```
5.  **Run the development server:**
    ```sh
    npm run dev
    ```
    Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

---

## Deployment

This application is designed for easy deployment on [Vercel](https://vercel.com/).

1.  Push your code to your GitHub repository.
2.  Sign up or log in to Vercel using your GitHub account.
3.  Import your GitHub repository into Vercel.
4.  **Crucially**, add all the environment variables from your `.env.local` file to the Vercel project settings.
5.  Deploy! Vercel will handle the rest.
