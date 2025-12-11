**EBankc - DeFi Banking Platform 🏦**

EBankc is a modern Next.js web application designed for a Decentralized Finance (DeFi) banking platform. It serves as the frontend interface for users to explore crypto assets, earn interest, borrow against holdings, and learn about the ecosystem via a blog and FAQ.

🚀 Key Features

Responsive UI/UX: Fully responsive design featuring a custom mobile menu and smooth transitions using Framer Motion.

Dynamic Blog System: A blog section with tagging support, main feature posts, and individual post routing (/blog/post/[id]).

Asset & Data Visualization: Custom components to display crypto asset growth, token statistics, and complex data tables (Karma Levels).

SEO Optimized: Integrated Next-SEO for managing Open Graph tags, titles, and meta descriptions across all pages.

Informational Pages: Dedicated sections for Corporate clients, Token utility (EBCT), Statistics, and Company background.

FAQ System: an interactive, categorized Frequently Asked Questions section.

🛠️ Tech Stack

Framework: Next.js (Pages Router)

Library: React

Styling: Sass / SCSS Modules

Animations: Framer Motion

SEO: next-seo

📂 Project Structure
```bash
├── components/          # Reusable UI components
│   ├── Asset.jsx        # Crypto asset card display
│   ├── BlogPost.jsx     # Blog post card (Main and Mini variants)
│   ├── Footer.jsx       # Global application footer
│   ├── Navbar.jsx       # Responsive navigation bar with Mobile Menu
│   └── Table.jsx        # Data table for Karma/Reward levels
├── pages/               # Application routes
│   ├── blog/            # Blog listing, tags, and dynamic post pages
│   ├── faq/             # FAQ listing and section views
│   ├── _app.js          # Global entry point (SEO & Global styles)
│   ├── index.js         # Homepage
│   ├── corporates.js    # B2B/Corporate landing page
│   ├── token.js         # EBCT Token utility info
│   └── stats.js         # Platform statistics
├── styles/              # SCSS Modules and Global styles
└── public/              # Static assets (images, icons)
```

⚡ Getting Started

Follow these instructions to get a copy of the project up and running on your local machine.

Prerequisites

Node.js (v14 or newer)

npm or yarn

Installation

Clone the repository:

```bash
git clone https://github.com/Brkic365/ebankc-defi.git
cd ebankc-defi
```

Install dependencies:

```bash
npm install
# or
yarn install
```

Run the development server:

```bash
npm run dev
```

Open http://localhost:3000 with your browser to see the result.

📖 Component Highlights
Karma Table (Table.jsx)

A specialized component designed to display reward tiers. It handles complex grid layouts to show how holding EBCT tokens increases APY rates for different assets.

Navigation (Navbar.jsx)

Includes a framer-motion powered sidebar for mobile devices. It automatically highlights the active link and creates an animated underline effect for the current page.

Blog System (pages/blog/)

Currently utilizes local data arrays to render posts. It supports:

Main Post: A featured article at the top.

Sub Posts: Secondary highlighted articles.

Tag Filtering: Filter posts via query parameters (e.g., /blog/tag?q=DeFi).

🔮 Future Improvements

CMS Integration: Connect the Blog and Team sections to a Headless CMS (like Contentful or Strapi) instead of using hardcoded arrays.

Live Data: Connect the stats.js and token.js pages to a real Crypto API (like CoinGecko) to fetch real-time EBCT prices and market caps.

Authentication: Integrate the Login/Signup buttons with a backend auth provider.

📄 License

This project is open source and available under the MIT License.
