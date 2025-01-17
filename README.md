<div align="center">
    <a href="https://horizon-bank-fv.vercel.app" target="_blank">
      <img src="public/design/preview.png" alt="Project Banner">
    </a>
  <h3 align="center">Banking Platform</h3>
</div>

##  <br /> 📋 <a name="table">Table of Contents</a>

- ✨ [Introduction](#introduction)
- ⚙️ [Tech Stack](#tech-stack)
- 📝 [Features](#features)
- 🚀 [Quick Start](#quick-start)

##  <br /> <a name="introduction">✨ Introduction</a>

**[EN]** Built with Next.js, Horizon is a financial SaaS platform that connects to multiple bank accounts, displays transactions in real-time, allows users to transfer money to other platform users, and manages their finances altogether.

**[FR]** Construit avec Next.js, Horizon est une plateforme SaaS financière qui se connecte à plusieurs comptes bancaires, affiche les transactions en temps réel, permet aux utilisateurs de transférer de l'argent à d'autres utilisateurs de la plateforme et gère leurs finances de manière globale.

##  <br /> <a name="tech-stack">⚙️ Tech Stack</a>

- [**Next.js**](https://nextjs.org/docs) is a React framework for building high-performance web applications with server-side rendering (SSR) and static site generation (SSG). It optimizes SEO and provides features like automatic code splitting, API routes, and an extensive plugin ecosystem.

- [**React**](https://react.dev/reference/react) is a JavaScript library for building user interfaces. React allows developers to create reusable UI components and manage the state efficiently. It is known for its virtual DOM and component-based architecture, which enhances performance and maintainability.

- [**TypeScript**](https://www.typescriptlang.org/docs/) is a statically typed superset of JavaScript that adds type definitions to enhance code maintainability and robustness. It helps developers catch errors early in the development process and provides better tooling and refactoring capabilities.

- [**Appwrite**](https://appwrite.io/docs) is an open-source backend server that provides essential services like authentication, real-time databases, file storage, cloud functions, and more. It's designed to streamline web and mobile app development by offering a unified API for backend functionalities.

- [**Plaid**](https://plaid.com/docs/) is a financial services API that allows applications to connect with users' bank accounts, retrieve transaction data, verify account balances, and access other banking information. It supports integrations with major banks and financial institutions, enhancing fintech applications.

- [**Dwolla**](https://developers.dwolla.com/docs)  is a payments platform that enables businesses to integrate ACH (Automated Clearing House) payments for transferring money between bank accounts. It offers features like real-time payments, low transaction fees, and robust security measures, making it suitable for various payment solutions.

- [**React Hook Form**](https://react-hook-form.com/docs) is a library for managing form state and validation in React applications. It leverages React hooks to provide a minimal API, improving form performance and reducing the amount of code needed for complex form handling and validation.

- [**Zod**](https://zod.dev/)  is a TypeScript-first schema declaration and validation library that ensures data integrity and validation through its strong typing and inference capabilities. Zod allows developers to define schemas for their data models, providing runtime validation and type safety.

- [**Tailwind**](https://v2.tailwindcss.com/docs) is a utility-first CSS framework for rapidly building custom user interfaces. It offers a comprehensive set of utility classes that can be composed to create complex designs without writing custom CSS. TailwindCSS promotes consistency and reusability in styling.

- [**Chart.js**](https://www.chartjs.org/docs/latest/getting-started/)  is a flexible JavaScript charting library for creating interactive and visually appealing charts and graphs. It supports various chart types, such as line, bar, pie, and radar charts, and offers extensive customization options to tailor the visual representation to specific needs.

- [**shadcn/ui**](https://ui.shadcn.com/docs) is a component library that provides a set of highly customizable components designed to work seamlessly with React and TailwindCSS. ShadCN focuses on delivering accessible, reusable, and themeable components to accelerate UI development and maintain design consistency.

## <br/> <a name="features">📝 Features</a>

👉 **Authentication**: An ultra-secure SSR authentication with proper validations and authorization

👉 **Connect Banks**: Integrates with Plaid for multiple bank account linking

👉 **Home Page**: Shows general overview of user account with total balance from all connected banks, recent transactions, money spent on different categories, etc

👉 **My Banks**: Check the complete list of all connected banks with respective balances, account details

👉 **Transaction History**: Includes pagination and filtering options for viewing transaction history of different banks

👉 **Real-time Updates**: Reflects changes across all relevant pages upon connecting new bank accounts.

👉 **Funds Transfer**: Allows users to transfer funds using Dwolla to other accounts with required fields and recipient bank ID.

👉 **Responsiveness**: Ensures the application adapts seamlessly to various screen sizes and devices, providing a consistent user experience across desktop, tablet, and mobile platforms.

## <br /> <a name="quick-start">🚀 Quick Start</a>

Follow these steps to set up the project locally on your machine.

<br/>**Prerequisites**

Make sure you have the following installed on your machine:

- [Git](https://git-scm.com/)
- [Node.js](https://nodejs.org/en)
- [npm](https://www.npmjs.com/) (Node Package Manager)

<br/>**Cloning the Repository**

```bash
git clone {git remote URL}
```

<br/>**Installation**

Let's install the project dependencies, from your terminal, run:

```bash
npm install
# or
yarn install
```

<br/>**Set Up Environment Variables**

Create a new file named `.env` in the root of your project and add the following content:

```env
# Change this one with deployment URL!
NEXT_PUBLIC_SITE_URL=http://localhost:3000

# Appwrite
NEXT_PUBLIC_APPWRITE_ENDPOINT=https://cloud.appwrite.io/v1
NEXT_PUBLIC_APPWRITE_PROJECT=
APPWRITE_DATABASE_ID=
APPWRITE_USER_COLLECTION_ID=
APPWRITE_BANK_COLLECTION_ID=
APPWRITE_TRANSACTION_COLLECTION_ID=
NEXT_APPWRITE_KEY=

# Plaid
PLAID_CLIENT_ID=
PLAID_SECRET=
PLAID_ENV=sandbox
PLAID_PRODUCTS=auth,transactions,identity
PLAID_COUNTRY_CODES=US,CA

# Dwolla
DWOLLA_KEY=
DWOLLA_SECRET=
DWOLLA_BASE_URL=https://api-sandbox.dwolla.com
DWOLLA_ENV=sandbox
```

Replace the placeholder values with your actual respective account credentials:

- [Appwrite](https://cloud.appwrite.io)
- [Plaid](https://dashboard.plaid.com/overview)
- [Dwolla](https://dashboard.plaid.com/overview)



<br/>**Running the Project**

Installation will take a minute or two, but once that's done, you should be able to run the following command:

```bash
npm run dev
# or
yarn dev
```

Open [`http://localhost:3000`](http://localhost:3000) in your browser to view the project.

<br/>**Test User**
- Email : john@mail.com
- Password : johnjohn


