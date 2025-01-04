# Comfy Store Documentation

## Project Overview

**Comfy Store** is a modern e-commerce web application designed for both mobile and tablet devices. This project leverages **Next.js** for building a fast and responsive user interface, utilizes **Prisma** and **Supabase** for data management, and provides secure user authentication via **Clerk**.

The platform allows guests to browse products but limits permissions for actions such as adding items to the shopping cart, placing orders, leaving reviews, and accessing order history. To unlock these functionalities, users need to register for an account.

## Key Features

### User Roles

1. **Guest Users**:

   - Can view products on the site.
   - Cannot make purchases, add items to their shopping cart, leave reviews, or access order history.

2. **Registered Users**:

   - Can register easily using their email, Google, or GitHub accounts.
   - Gain access to functionalities such as:
     - Shopping cart for managing product selections
     - Favorites feature to save preferred items
     - Ability to leave reviews on purchased products
     - View order history and track current orders

3. **Admin Users**:
   - Have access to the admin panel to manage the store.
   - Can perform actions such as:
     - Adding new products to the database
     - Editing existing products
     - Monitoring inventory levels and sales data

### Authentication

The application uses **Clerk** for user authentication, providing a seamless sign-up and login experience. Users can easily register via email, Google, or GitHub, making the process straightforward and user-friendly.

### Product Management

Admin users can manage the product catalog through the admin panel which includes:

- Creating new products in the database.
- Editing existing products to update details or prices.
- Tracking sales and inventory to ensure the store is well-managed.

### Payment Integration

The application supports secure payments through **Stripe**, allowing users to pay for their orders safely. This integration ensures that all transactions are smooth and secure.

### Technology Stack

The project is built using the following technologies:

- **Framework**: [Next.js](https://nextjs.org/)
- **Database Management**: [Prisma](https://www.prisma.io/) and [Supabase](https://supabase.io/)
- **Authentication**: [Clerk](https://clerk.dev/)
- **Payment Processing**: [Stripe](https://stripe.com/)
- **State Management and UI Components**: Various packages including **Radix UI** and **Tailwind CSS** for styling.

## Project Setup

To run the project locally, follow these steps:

### 1. Clone the Repository

To copy the project from GitHub to your local machine, open your terminal and run the following command:

```bash
git clone https://github.com/yourusername/comfy-store.git
Make sure to replace yourusername with the actual username of the repository owner on GitHub.

2. Navigate to the Project Directory
Change to the project directory:

bash

cd comfy-store
3. Install Dependencies
Install the necessary dependencies using npm:

bash

npm install
4. Set Up Environment Variables
Create a .env.local file in the root of the project and add your environment variables. You will need to set your Stripe keys and Clerk API keys. Example:

plaintext

NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=your_publishable_key
STRIPE_SECRET_KEY=your_secret_key
CLERK_API_KEY=your_clerk_api_key
Make sure to replace the placeholders with your actual credentials.

5. Run the Application
To start the application in development mode, run:

bash

npm run dev
6. Build for Production (Optional)
If you wish to build the application for production, run:

bash

npm run build
7. Start the Production Server (Optional)
To start the application in production mode, run:

bash

npm run start
Scripts
Here are the important scripts defined in the package.json:

dev: Runs the application in development mode.
build: Generates the Prisma client and builds the application.
start: Starts the application in production mode.
lint: Lints the codebase for style and quality issues.
Dependencies
This project utilizes various dependencies, including but not limited to:

@clerk/nextjs: For user authentication.
@prisma/client: For database client operations.
@stripe/react-stripe-js: For integrating Stripe payments.
axios: For making HTTP requests.
zod: For input validation during product creation.
Conclusion
The Comfy Store project delivers a robust e-commerce experience for both customers and administrators. With its user-friendly interface and powerful backend capabilities, it is designed to provide an effective online shopping solution. Whether you're browsing as a guest or managing products as an admin, Comfy Store aims to meet the needs of all users in the ever-growing world of online retail.

For further inquiries or contributions, please reach out or check the project repository.
```
