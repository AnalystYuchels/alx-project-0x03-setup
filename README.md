# alx-project-0x02-setup

![License](https://img.shields.io/badge/license-MIT-green.svg)
![TypeScript](https://img.shields.io/badge/language-TypeScript-blue)
![TailwindCSS](https://img.shields.io/badge/styling-TailwindCSS-38B2AC)
![Next.js](https://img.shields.io/badge/framework-Next.js-black)
![Status](https://img.shields.io/badge/status-In%20Progress-yellow)

## 📚 Project Overview

This project is a user listing app built with **Next.js**, **TypeScript**, and **TailwindCSS**. It fetches and displays user data from an external API using reusable components and organized modular files.

The goal is to demonstrate key frontend concepts, such as component reusability, API data fetching, and strict typing in TypeScript, within a modern web development stack.


## 🎯 Learning Objectives

- Understand the file structure and organization of a Next.js TypeScript project.
- Build and reuse functional components like cards and layouts.
- Interface with APIs using `getServerSideProps` for data fetching.
- Apply strict typing with custom interfaces (`UserProps`, etc.).
- Use TailwindCSS for responsive and modern UI styling.
- Handle layout separation (header/footer/main) using layout wrappers.


## 🧱 Project Structure

```bash
.
├── components/               # Reusable UI components
│   ├── common/              # Shared elements across pages (e.g. UserCard)
│   └── layout/              # Layout-related components like Header, Footer
│
├── interfaces/              # TypeScript interfaces for props & data
│   └── index.ts             # Contains UserProps interface for typing user data
│
├── pages/                   # Next.js pages
│   ├── _app.tsx            # Entry point for global styles/wrappers
│   └── users.tsx           # Main page that displays users fetched from API
│
├── public/                  # Static assets like images
│
├── styles/                  # TailwindCSS and global styles (if needed)
│   └── globals.css
│
├── tsconfig.json            # TypeScript config
├── tailwind.config.ts       # Tailwind configuration
└── next.config.js           # Next.js configuration
````


## 📦 Setup Instructions

1. **Clone the Repository**

```bash
git clone https://github.com/AnalystYuchels/alx-project-0x02-setup.git
cd alx-project-0x02-setup
```

2. **Install Dependencies**

```bash
npm install
# or
yarn
```

3. **Run the Development Server**

```bash
npm run dev
# or
yarn dev
```

4. Open [http://localhost:3000/users](http://localhost:3000/users) in your browser to view the app.


## 🧠 How It Works

* `interfaces/index.ts`: Defines a `UserProps` interface which strongly types each user’s data (name, email, address).
* `components/common/UserCard.tsx`: A reusable component that displays individual user data in a styled card.
* `pages/users.tsx`:

  * Uses `getServerSideProps()` to fetch user data from an external API.
  * Maps over the fetched users and displays each in a `UserCard`.


## 🌟 Features

* Responsive UI using TailwindCSS utility classes.
* Clear type safety with TypeScript interfaces.
* Modular folder structure separating concerns.
* Reusable and scalable component design.
* API integration via `getServerSideProps` for SSR.
* Easy customization and extension for more features.


## 🧪 Testing the Application

### Core Functionality Tests:

Layout Consistency: Verify Header and Footer appear on all pages
Button Interactions: Test all button variants and click handlers
Font Loading: Confirm Montserrat font is applied globally
Routing: Test navigation between pages
404 Handling: Visit non-existent routes to see custom error page
Responsive Design: Test on different screen sizes

### Component Tests:

```bash
# Test button variants
- Click the "Sign In" and "Sign Up" buttons in the header
- Test navigation buttons on the landing page
- Verify hover effects and transitions

# Test routing
- Navigate to /unknown-page to see 404
- Use "Go Back Home" link on 404 page
- Test browser back/forward navigation
```


## 🛠️ Tools Used

* **Next.js** – React framework for building server-rendered apps.
* **TypeScript** – For strict typing and interface definitions.
* **TailwindCSS** – For styling components using utility classes.
* **Fetch API** – For getting user data from an external endpoint.


## 🚀 Deployment

To deploy this project using **Vercel**:

1. Push your code to GitHub.
2. Visit [vercel.com](https://vercel.com).
3. Link your GitHub repository.
4. Set up build command (default is fine: `npm run build`) and root directory.
5. Click **Deploy**.


## 🧾 License

This project is licensed under the **MIT License** – feel free to use and modify it.


## ✅ To Do

* [x] Set up folder structure
* [x] Add TailwindCSS and TypeScript support
* [x] Create `UserProps` interface
* [x] Build reusable `UserCard` component
* [x] Fetch and display API data on `/users` page
* [ ] Add loading/error states
* [ ] Implement pagination or filtering
* [ ] Add dark mode
