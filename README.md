# ALX Project 0x03 - Shared Layouts in Next.js

[![Next.js](https://img.shields.io/badge/Next.js-13+-blue.svg)](https://nextjs.org/)
[![TailwindCSS](https://img.shields.io/badge/TailwindCSS-%5E3.x-blue)](https://tailwindcss.com/)
[![React Icons](https://img.shields.io/badge/React%20Icons-%5E4.10.1-blue)](https://react-icons.github.io/react-icons/)

## 📌 Objective

In most real-world applications, multiple pages share common elements like headers and footers. This project demonstrates how to avoid redundancy using the **DRY (Don't Repeat Yourself)** principle by creating reusable layout components in a Next.js app.


## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/AnalystYuchels/alx-project-0x03-setup.git
cd alx-project-0x03-setup
````

### 2. Install dependencies

```bash
npm install
```

### 3. Run the development server

```bash
npm run dev
```

Open your browser and visit:
👉 [http://localhost:3000](http://localhost:3000)


## 🏗️ Project Structure

```bash
alx-project-0x03/
│
├── components/
│   ├── common/
│   │   └── Button.tsx             # Reusable button component with props
│   └── layouts/
│       ├── Header.tsx             # Top navigation with Sign In/Up buttons
│       ├── Footer.tsx             # Bottom section with links and social icons
│       └── Layout.tsx             # Wraps all pages with Header and Footer
│
├── interfaces/
│   └── index.ts                   # All shared TypeScript interfaces
│
├── pages/
│   ├── 404.tsx                    # Custom 404 error page
│   └── index.tsx                  # Landing page with imperative routing
│
├── public/                        # Static files (e.g. favicon)
│
├── styles/
│   └── globals.css                # TailwindCSS setup and Google Fonts
│
├── tsconfig.json                  # TypeScript configuration
└── next.config.js                 # Next.js configuration
```


## ✨ Features

* **Shared Layouts** using `Layout.tsx`
* **Modular components** (Header, Footer, Button)
* **Google Fonts** integrated (Montserrat)
* **Imperative Routing** using `useRouter` hook
* **Type-safe Interfaces** managed under `/interfaces`
* **Custom 404 Page** with a fun message
* **TailwindCSS Styling** for fast and clean UI


## 🧩 Components Breakdown

### `Button.tsx`

* Reusable with support for custom text, size, color, and actions.

### `Header.tsx`

* Fixed top navigation with logo and Sign In/Up buttons.

### `Footer.tsx`

* Contains description, useful links, and social icons (Facebook, Twitter, Instagram).

### `Layout.tsx`

* Wraps each page with `<Header />`, `<Footer />`, and `<main>{children}</main>`.


## 🛠️ Tech Stack

* [Next.js](https://nextjs.org/)
* [React](https://reactjs.org/)
* [TypeScript](https://www.typescriptlang.org/)
* [TailwindCSS](https://tailwindcss.com/)
* [React Icons](https://react-icons.github.io/react-icons/)
* [Google Fonts - Montserrat](https://fonts.google.com/specimen/Montserrat)


## 🧪 Testing

After setup, run:

```bash
npm run dev
```

* Visit `/` to see the welcome page.
* Try navigating using the buttons — you’ll hit a custom 404 page since routes are placeholders.
* Visit `/unknown-pathname` to preview the custom error screen.


## ✅ Learning Outcomes

* DRY principle using layout components
* Building reusable UI components
* Implementing imperative navigation
* Managing global styles and fonts
* Handling 404 errors gracefully
* Organizing TypeScript interfaces


## 👨‍💻 Author

**Uchechi Uche** — [@AnalystYuchels](https://github.com/AnalystYuchels)


## 📄 License

This project is part of the **ALX Frontend Program** and is intended for educational purposes.
