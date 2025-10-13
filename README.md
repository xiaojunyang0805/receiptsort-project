# ReceiptSort Project

> AI-powered receipt management system with automated OCR, categorization, and export capabilities.

[![Project Status](https://img.shields.io/badge/status-active-success.svg)]()
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

## 📋 Overview

ReceiptSort is a comprehensive receipt management solution that uses AI to automatically extract, categorize, and organize receipt data. This repository serves as the central hub for all public components and documentation.

## 🏗️ Project Structure

This project consists of multiple repositories:

### Public Repositories (Open Source)

#### 1. [receiptsort-ui](https://github.com/xiaojunyang0805/receiptsort-ui)
**Reusable React UI Components Library**

- 20+ production-ready components built with shadcn/ui
- Full TypeScript support
- Tailwind CSS styling
- Components: Button, Card, Dialog, Form, Input, Select, Table, Tabs, Toast, and more

```bash
npm install @receiptsort/ui
```

[View Repository →](https://github.com/xiaojunyang0805/receiptsort-ui)

#### 2. [receiptsort-landing](https://github.com/xiaojunyang0805/receiptsort-landing)
**Modern Landing Page Template**

- Animated hero section with gradient backgrounds
- Feature showcase grid
- Step-by-step "How It Works" visualization
- FAQ and testimonials sections
- Multi-language support (i18n)
- Built with Next.js 15 and React 18

[View Repository →](https://github.com/xiaojunyang0805/receiptsort-landing)

#### 3. [receiptsort-utils](https://github.com/xiaojunyang0805/receiptsort-utils)
**Utility Functions & React Hooks**

- `cn()` - Smart className merger for Tailwind CSS
- `useToast()` - Toast notification hook
- TypeScript utilities for common patterns

```bash
npm install @receiptsort/utils
```

[View Repository →](https://github.com/xiaojunyang0805/receiptsort-utils)

### Private Repository

#### receiptsort (Main Application)
**Production Application** - Contains the full receipt management system with:
- AI-powered OCR using OpenAI
- Receipt processing and categorization
- Export to Excel/CSV
- Credit system and subscriptions
- User authentication
- Dashboard and management features

*This repository is private and contains proprietary business logic.*

## 🚀 Features

- **AI-Powered OCR** - Automatic receipt data extraction using advanced AI
- **Smart Categorization** - Intelligent categorization of expenses
- **Multi-Format Export** - Export to Excel, CSV with customizable templates
- **Batch Processing** - Process multiple receipts at once
- **Multi-Language** - Support for English, Chinese, Japanese, Korean, and more
- **Responsive Design** - Works seamlessly on desktop and mobile
- **Secure & Private** - Your data stays protected

## 🛠️ Tech Stack

### Frontend
- **Next.js 15** - React framework with App Router
- **React 18** - UI library
- **TypeScript** - Type safety
- **Tailwind CSS** - Styling
- **shadcn/ui** - Component library
- **next-intl** - Internationalization

### Backend & Services
- **Supabase** - Database and authentication
- **OpenAI API** - OCR and data extraction
- **Stripe** - Payment processing
- **Vercel** - Hosting and deployment

### Tools & Libraries
- **ExcelJS** - Excel file generation
- **Papa Parse** - CSV parsing
- **Lucide React** - Icons
- **date-fns** - Date utilities

## 📦 Installation

### Using the Components

```bash
# Install UI components
npm install @receiptsort/ui

# Install utilities
npm install @receiptsort/utils
```

### Running the Landing Page Locally

```bash
# Clone the landing page repo
git clone https://github.com/xiaojunyang0805/receiptsort-landing.git
cd receiptsort-landing

# Install dependencies
npm install

# Run development server
npm run dev
```

## 🎯 Use Cases

- **Individuals** - Track personal expenses and receipts
- **Freelancers** - Manage business expenses for tax purposes
- **Small Businesses** - Organize company receipts and reimbursements
- **Accountants** - Streamline receipt processing for clients

## 📚 Documentation

- [UI Components Documentation](https://github.com/xiaojunyang0805/receiptsort-ui#readme)
- [Landing Page Guide](https://github.com/xiaojunyang0805/receiptsort-landing#readme)
- [Utilities API Reference](https://github.com/xiaojunyang0805/receiptsort-utils#readme)

## 🔗 Quick Links

| Repository | Description | Status | Topics |
|------------|-------------|--------|--------|
| [receiptsort-ui](https://github.com/xiaojunyang0805/receiptsort-ui) | UI Components | Public | `react` `typescript` `tailwind-css` |
| [receiptsort-landing](https://github.com/xiaojunyang0805/receiptsort-landing) | Landing Page | Public | `nextjs` `landing-page` `i18n` |
| [receiptsort-utils](https://github.com/xiaojunyang0805/receiptsort-utils) | Utilities & Hooks | Public | `react` `hooks` `typescript` |
| receiptsort | Main Application | Private | `full-stack` `ai` `saas` |

## 🔍 Finding All Related Repositories

To find all repositories related to this project, use GitHub search:

```
user:xiaojunyang0805 topic:receiptsort-project
```

Or click here: [View all receiptsort repositories](https://github.com/xiaojunyang0805?tab=repositories&q=topic%3Areceipt sort-project)

## 🤝 Contributing

Contributions to the public components are welcome! Please feel free to:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

The public components (UI, Landing, Utils) are licensed under the MIT License. See individual repository LICENSE files for details.

The main application (private repository) is proprietary software.

## 👤 Author

**xiaojunyang0805**

- GitHub: [@xiaojunyang0805](https://github.com/xiaojunyang0805)
- Email: xiaojunyang0805@gmail.com

## 🌟 Show Your Support

If you find these components useful, please consider:
- Giving a ⭐️ to the repositories
- Sharing with others who might find them helpful
- Contributing improvements

## 📝 Changelog

### Version 1.0.0 (2025-10-13)
- Initial public release
- Published UI components library
- Published landing page template
- Published utilities package
- Created project hub repository

## 🔮 Roadmap

- [ ] Add Storybook for UI components
- [ ] Create demo site for landing page
- [ ] Publish packages to npm
- [ ] Add more utility functions
- [ ] Create video tutorials
- [ ] Add component screenshots

## ❓ FAQ

**Q: Can I use these components in my commercial project?**
A: Yes! The public components are MIT licensed and free to use in any project.

**Q: Is the main ReceiptSort application open source?**
A: No, the main application is proprietary. Only the reusable components are open source.

**Q: How do I report bugs or request features?**
A: Please open an issue in the specific repository (UI, Landing, or Utils).

**Q: Are you accepting contributions?**
A: Yes! Contributions to the public components are welcome.

## 📧 Contact

For questions, suggestions, or collaboration opportunities, feel free to reach out!

---

<p align="center">
  Made with ❤️ by xiaojunyang0805
</p>

<p align="center">
  <a href="https://github.com/xiaojunyang0805/receiptsort-ui">UI Components</a> •
  <a href="https://github.com/xiaojunyang0805/receiptsort-landing">Landing Page</a> •
  <a href="https://github.com/xiaojunyang0805/receiptsort-utils">Utilities</a>
</p>
