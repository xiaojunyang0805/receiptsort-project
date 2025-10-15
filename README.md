# ReceiptSort Project

> AI-powered receipt management system with automated OCR, categorization, and comprehensive data extraction for personal, business, and medical receipts.

[![Project Status](https://img.shields.io/badge/status-active-success.svg)]()
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Live Demo](https://img.shields.io/badge/demo-live-brightgreen.svg)](https://receiptsort.seenano.nl)

## 🌐 Live Application

**Try ReceiptSort now:** [https://receiptsort.seenano.nl](https://receiptsort.seenano.nl)

The production application is live and features:
- ✅ AI-powered receipt data extraction (22 fields)
- ✅ Medical receipt support for insurance reimbursement
- ✅ Business invoice line items (QuickBooks/Xero compatible)
- ✅ Smart document type detection
- ✅ 7 language support (English, Dutch, German, French, Spanish, Japanese, Chinese)
- ✅ All image formats supported (PNG, JPEG, GIF, BMP, TIFF, PDF, WebP)

## 📋 Overview

ReceiptSort is a comprehensive receipt management solution that uses AI to automatically extract, categorize, and organize receipt data. This repository serves as the central hub for all public components and documentation.

**Latest Update (October 2025):** Market Value Enhancement Phase completed with 14 new fields for medical receipts and business invoices.

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
**Production Application** - [https://receiptsort.seenano.nl](https://receiptsort.seenano.nl)

Contains the full receipt management system with:
- AI-powered OCR using OpenAI GPT-4o
- Receipt processing and categorization
- Export to Excel/CSV (22 columns)
- Medical receipt support (insurance reimbursement)
- Business invoice line items
- Credit system and subscriptions
- User authentication (Google OAuth + email/password)
- Dashboard and management features
- Multi-language support (7 languages)

*This repository is private and contains proprietary business logic.*

## 🚀 Features

### Core Features
- **AI-Powered OCR** - Automatic receipt data extraction using OpenAI GPT-4o
- **Smart Categorization** - Intelligent categorization of expenses
- **Multi-Format Export** - Export to Excel, CSV with 22 columns of data
- **Batch Processing** - Process multiple receipts at once
- **Multi-Language** - Support for 7 languages (EN, NL, DE, FR, ES, JA, ZH)
- **Responsive Design** - Works seamlessly on desktop and mobile
- **Secure & Private** - Your data stays protected with Supabase RLS

### Advanced Data Extraction (22 Fields)

#### Basic Receipt Data (8 fields)
- Merchant name, total amount, currency, date
- Category, tax amount, payment method, notes

#### Phase 1: Essential Fields (5 fields)
- **Invoice Number** - Critical for medical insurance reimbursement
- **Document Type** - Auto-detected (receipt, invoice, medical_invoice, bill)
- **Subtotal** - Amount before tax
- **Vendor Address** - Full vendor address
- **Due Date** - Payment due date

#### Phase 2: Business Invoices (3 fields + line items)
- **Purchase Order Number** - PO number for business invoices
- **Payment Reference** - Transaction ID, check number
- **Vendor Tax ID** - VAT/Tax ID/EIN/BTW number
- **Line Items Table** - Line-by-line invoice breakdown with:
  - Line number, description, quantity
  - Unit price, line total, item code
  - Tax rate per line

#### Phase 3: Medical Receipts (6 fields)
- **Patient Date of Birth** - Patient DOB
- **Treatment Date** - Actual service date (separate from invoice date)
- **Insurance Claim Number** - Insurance claim reference
- **Diagnosis Codes (ICD)** - Medical diagnosis codes (comma-separated)
- **Procedure Codes (CPT)** - Treatment/procedure codes (comma-separated)
- **Provider ID (AGB/NPI)** - Healthcare provider identification

### Smart Features
- **Document Type Detection** - Automatically identifies receipts, invoices, medical invoices, bills
- **Conditional UI** - Shows only relevant fields based on document type
- **Image Format Support** - PNG, JPEG, GIF, BMP, TIFF, PDF, WebP (with automatic conversion)
- **QuickBooks/Xero Compatible** - Line items and tax IDs for accounting software integration

## 🛠️ Tech Stack

### Frontend
- **Next.js 15** - React framework with App Router
- **React 18** - UI library
- **TypeScript** - Type safety
- **Tailwind CSS** - Styling
- **shadcn/ui** - Component library
- **next-intl** - Internationalization

### Backend & Services
- **Supabase** - PostgreSQL database and authentication
- **OpenAI GPT-4o** - OCR and data extraction
- **Stripe** - Payment processing
- **Vercel** - Hosting and deployment

### Tools & Libraries
- **ExcelJS** - Excel file generation (with auto-filter, formatting)
- **Papa Parse** - CSV parsing
- **Sharp & Jimp** - Image format conversion
- **pdf-parse-fork** - PDF text extraction
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

### For Individuals
- Track personal expenses and receipts
- Prepare tax documents with detailed records
- Organize household bills and invoices

### For Medical Patients
- **Insurance Reimbursement** - Extract patient info, claim numbers, diagnosis codes
- Healthcare expense tracking with treatment dates
- Medical record organization with procedure codes and provider IDs
- Compliant with medical billing standards (ICD/CPT codes)

### For Freelancers & Small Businesses
- Manage business expenses for tax purposes
- Track invoices with line item details
- Purchase order tracking and payment reconciliation
- **QuickBooks/Xero Integration** - Export with line items, tax IDs, subtotals

### For Accountants
- Streamline receipt processing for clients
- Generate detailed expense reports with 22 data fields
- Audit trail support with full invoice details
- Batch processing for multiple clients

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

## 🎨 Live Demo & Screenshots

**Visit the live application:** [https://receiptsort.seenano.nl](https://receiptsort.seenano.nl)

Features you can try:
- Upload receipts (drag & drop or file picker)
- Auto-processing with AI extraction
- View extracted data in receipt details
- Export to CSV/Excel with 22 columns
- Multi-language interface (switch between 7 languages)

## 🚀 Recent Updates

### Version 2.0.0 (October 2025) - Market Value Enhancement
**Major update with 14 new data fields**

- ✅ **Phase 1: Essential Fields** (5 fields)
  - Invoice numbers, document types, subtotals, vendor addresses, due dates

- ✅ **Phase 2: Business Invoices** (3 fields + line items)
  - Purchase orders, payment references, tax IDs
  - Line items table with 7 fields per line

- ✅ **Phase 3: Medical Receipts** (6 fields)
  - Patient DOB, treatment dates, insurance claims
  - Diagnosis codes (ICD), procedure codes (CPT), provider IDs (AGB/NPI)

- ✅ **Enhanced AI Extraction**
  - 200+ lines of extraction rules
  - Smart document type detection
  - Medical terminology recognition

- ✅ **Conditional UI**
  - Shows only relevant fields based on document type
  - 3 new UI sections (Invoice Details, Business Invoice, Medical Information)

- ✅ **Export Improvements**
  - 22-column CSV/Excel exports (up from 8 columns)
  - Proper date formatting, currency formatting
  - Auto-filter support

### Version 1.0.0 (October 2025) - Initial Launch
- Initial public release
- Published UI components library
- Published landing page template
- Published utilities package
- Created project hub repository

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

**Xiaojun Yang**

- GitHub: [@xiaojunyang0805](https://github.com/xiaojunyang0805)
- Email: xiaojunyang0805@gmail.com
- Company: Seenano Technology B.V.
- Website: [https://receiptsort.seenano.nl](https://receiptsort.seenano.nl)

## 🌟 Show Your Support

If you find these components useful, please consider:
- Giving a ⭐️ to the repositories
- Trying the live app at [receiptsort.seenano.nl](https://receiptsort.seenano.nl)
- Sharing with others who might find them helpful
- Contributing improvements

## 🔮 Roadmap

### Completed
- [x] Add comprehensive data extraction (22 fields)
- [x] Medical receipt support (insurance reimbursement)
- [x] Business invoice line items
- [x] Smart document type detection
- [x] 7 language support
- [x] All image format support (PNG, JPEG, GIF, BMP, TIFF, PDF, WebP)
- [x] Production deployment (https://receiptsort.seenano.nl)

### In Progress
- [ ] Performance monitoring and analytics
- [ ] User feedback collection system

### Planned
- [ ] Add Storybook for UI components
- [ ] Create demo site for landing page
- [ ] Publish packages to npm
- [ ] Add more utility functions
- [ ] Create video tutorials
- [ ] Add component screenshots
- [ ] Mobile app (React Native)
- [ ] API for third-party integrations

## ❓ FAQ

**Q: Where can I try ReceiptSort?**
A: Visit [https://receiptsort.seenano.nl](https://receiptsort.seenano.nl) to try the live application!

**Q: What file formats are supported?**
A: We support PNG, JPEG, GIF, BMP, TIFF, PDF, and WebP. Images are automatically converted if needed.

**Q: Can ReceiptSort extract medical receipt data for insurance reimbursement?**
A: Yes! We extract patient DOB, treatment dates, insurance claim numbers, diagnosis codes (ICD), procedure codes (CPT), and provider IDs (AGB/NPI).

**Q: Is ReceiptSort compatible with accounting software like QuickBooks or Xero?**
A: Yes! We export line items, purchase orders, payment references, vendor tax IDs, and subtotals in a format compatible with accounting software.

**Q: How many languages are supported?**
A: We support 7 languages: English, Dutch, German, French, Spanish, Japanese, and Simplified Chinese.

**Q: Can I use the public components in my commercial project?**
A: Yes! The public components are MIT licensed and free to use in any project.

**Q: Is the main ReceiptSort application open source?**
A: No, the main application is proprietary. Only the reusable components (UI, Landing, Utils) are open source.

**Q: How do I report bugs or request features?**
A: For the live app, use the contact form at [receiptsort.seenano.nl/contact](https://receiptsort.seenano.nl/contact). For the public components, open an issue in the specific repository (UI, Landing, or Utils).

**Q: Are you accepting contributions?**
A: Yes! Contributions to the public components are welcome.

## 📧 Contact

For questions, suggestions, or collaboration opportunities:

- **Email:** support@seenano.nl
- **Contact Form:** [receiptsort.seenano.nl/contact](https://receiptsort.seenano.nl/contact)
- **GitHub Issues:** Open an issue in the relevant repository

---

<p align="center">
  Made with ❤️ in the Netherlands by Seenano Technology B.V.
</p>

<p align="center">
  <a href="https://receiptsort.seenano.nl">🌐 Live Demo</a> •
  <a href="https://github.com/xiaojunyang0805/receiptsort-ui">UI Components</a> •
  <a href="https://github.com/xiaojunyang0805/receiptsort-landing">Landing Page</a> •
  <a href="https://github.com/xiaojunyang0805/receiptsort-utils">Utilities</a>
</p>
