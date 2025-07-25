# Next.js Layout and Routing Project

## 🎯 Project Overview

This project demonstrates advanced Next.js concepts including shared layouts, Google Fonts integration, imperative routing, and custom error pages. The "Splash App" showcases modern React patterns using the DRY (Don't Repeat Yourself) principle for reusable UI components.

## 🚀 Features

- **Shared Layout System**: Reusable Header and Footer components across all pages
- **Custom Button Component**: Flexible button with multiple color options and sizes
- **Google Fonts Integration**: Beautiful Montserrat font applied globally
- **Imperative Routing**: Programmatic navigation using Next.js useRouter hook
- **Custom 404 Page**: Branded error page with user-friendly messaging
- **TypeScript Integration**: Full type safety with organized interfaces
- **Responsive Design**: Mobile-first approach with Tailwind CSS

## 🛠 Tech Stack

- **Framework**: Next.js 13+
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **Icons**: React Icons (Font Awesome)
- **Font**: Google Fonts (Montserrat)
- **Routing**: Next.js Pages Router with useRouter

## 📁 Project Structure

```
alx-project-0x03/
├── components/
│   ├── common/
│   │   └── Button.tsx           # Reusable button component
│   └── layouts/
│       ├── Header.tsx           # Navigation header
│       ├── Footer.tsx           # Site footer
│       └── Layout.tsx           # Main layout wrapper
├── interface/
│   └── index.ts                 # TypeScript interfaces
├── pages/
│   ├── 404.tsx                  # Custom error page
│   ├── _app.tsx                 # App wrapper
│   └── index.tsx                # Landing page
├── styles/
│   └── globals.css              # Global styles with fonts
├── package.json
├── tailwind.config.js
├── tsconfig.json
└── README.md
```

## 🎨 Components Overview

### Layout Components
- **Layout**: Main wrapper that includes Header and Footer
- **Header**: Fixed navigation with brand logo and action buttons
- **Footer**: Three-column footer with links and social media icons

### Common Components
- **Button**: Customizable button with size, color, and action properties

### Pages
- **Home**: Landing page with navigation to different app features
- **404**: Custom error page with friendly messaging and navigation

## 🔧 Getting Started

### Prerequisites
- Node.js (v16 or later)
- npm or yarn package manager
- Basic knowledge of React and TypeScript

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/alx-project-0x03-setup.git
cd alx-project-0x03-setup/alx-project-0x03
```

2. **Install dependencies**
```bash
npm install
# or
yarn install
```

3. **Install required packages**
```bash
npm install react-icons
```

4. **Run the development server**
```bash
npm run dev
# or
yarn dev
```

5. **Open in browser**
Navigate to [http://localhost:3000](http://localhost:3000)

## 🎯 Key Learning Objectives

### 1. **Shared Layout Pattern**
- Implementing DRY principle for consistent UI
- Creating reusable layout components
- Understanding component composition

### 2. **Google Fonts Integration**
- Adding external fonts to Next.js projects
- Global CSS configuration
- Typography best practices

### 3. **Imperative Routing**
- Using useRouter hook for programmatic navigation
- Difference between declarative and imperative routing
- Route parameters and navigation options

### 4. **Custom Error Handling**
- Creating branded 404 pages
- User experience improvements
- Error boundary concepts

### 5. **TypeScript Organization**
- Centralized interface management
- Type safety across components
- Import/export patterns

## 🎨 Styling Approach

### **Tailwind CSS Classes Used:**
- **Layout**: `container`, `mx-auto`, `flex`, `grid`
- **Spacing**: `py-`, `px-`, `mb-`, `gap-`
- **Colors**: `bg-blue-500`, `text-white`, `text-gray-800`
- **Responsive**: `md:`, `lg:` breakpoints
- **Effects**: `hover:`, `transition`, `shadow-md`

### **Component Variants:**
- Button colors: red, blue, orange, green
- Responsive grid layouts
- Mobile-first design approach

## 🔄 Routing System

### **Available Routes:**
- `/` - Landing page
- `/generate-text-ai` - Text generation feature (404 by design)
- `/text-to-image` - Image generation feature (404 by design)
- `/counter-app` - Counter application (404 by design)

### **Navigation Methods:**
- **Declarative**: Using Next.js `Link` component
- **Imperative**: Using `useRouter.push()` for programmatic navigation

## 🧪 Testing the Application

### **Core Functionality Tests:**
1. **Layout Consistency**: Verify Header and Footer appear on all pages
2. **Button Interactions**: Test all button variants and click handlers
3. **Font Loading**: Confirm Montserrat font is applied globally
4. **Routing**: Test navigation between pages
5. **404 Handling**: Visit non-existent routes to see custom error page
6. **Responsive Design**: Test on different screen sizes

### **Component Tests:**
```bash
# Test button variants
- Click "Sign In" and "Sign Up" buttons in header
- Test navigation buttons on landing page
- Verify hover effects and transitions

# Test routing
- Navigate to /unknown-page to see 404
- Use "Go Back Home" link on 404 page
- Test browser back/forward navigation
```

## 📝 Development Notes

### **Button Component Features:**
- **Props**: `buttonLabel`, `buttonSize`, `buttonBackgroundColor`, `action`
- **Color variants**: Dynamically applied Tailwind classes
- **Hover effects**: Semi-transparent hover states
- **Accessibility**: Proper button semantics

### **Layout System Benefits:**
- **Code Reusability**: Single layout definition for all pages
- **Maintenance**: Easy updates to header/footer across app
- **Consistency**: Unified user experience
- **Performance**: Shared components reduce bundle size

### **TypeScript Benefits:**
- **Type Safety**: Catch errors at compile time
- **IntelliSense**: Better development experience
- **Code Documentation**: Self-documenting interfaces
- **Refactoring**: Safe code changes with type checking

## 🔮 Future Enhancements

### **Potential Improvements:**
- Add theme switcher (dark/light mode)
- Implement actual AI features (text generation, image creation)
- Add user authentication system
- Include loading states and error boundaries
- Add unit and integration tests
- Implement SEO optimization
- Add internationalization (i18n)

### **Advanced Features:**
- Dynamic routing with parameters
- API routes for backend functionality
- Database integration
- State management with Context API or Redux
- Progressive Web App (PWA) features

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Next.js team for the amazing framework
- Tailwind CSS for utility-first styling
- React Icons for beautiful icon components
- Google Fonts for typography options
- ALX Africa for the project guidance

---

**Happy Coding! 🚀**

*This project demonstrates modern React and Next.js development patterns for building scalable web applications.*