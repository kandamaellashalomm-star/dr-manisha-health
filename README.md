# 🏥 Dr. Manisha Health — Premium E-Commerce Store

A beautiful, fully-functional e-commerce storefront for senior health supplements. Built with Next.js 15, PostgreSQL, and Drizzle ORM.

![Dr. Manisha Health](https://images.pexels.com/photos/6787542/pexels-photo-6787542.jpeg?auto=compress&cs=tinysrgb&fit=crop&h=300&w=800)

## ✨ Features

### 🛍️ Storefront
- **Stunning Home Page** — Hero section, animated #1 products showcase, featured collections
- **Product Catalog** — Grid with filters, sorting, search, and category navigation
- **Product Details** — Image galleries, reviews, benefits, ingredients, dosage info
- **Slide-out Cart** — Smooth animations, quantity controls, persistent state
- **Checkout Flow** — Multi-step form with order confirmation

### 💬 Live Chat Support
- Floating chat widget for customer support
- Real-time messaging with admin replies
- Session persistence across page refreshes

### ⚙️ Admin Dashboard (`/admin`)
- **Password Protected** — Secure access with password `IRANIUMMARKO123`
- **Product Management** — Add, edit, delete products
- **External Store Integration** — Import from Amazon, Shopify, Alibaba, eBay, Walmart, Etsy, AliExpress
- **Category Management** — Create and manage categories
- **Live Chat Panel** — Reply to customer messages in real-time

### 🎨 Premium Design
- Elegant emerald green + gold color scheme
- Playfair Display serif headings
- Smooth animations and transitions
- Fully responsive (mobile-first)
- Glass morphism effects

## 🚀 Tech Stack

- **Framework**: Next.js 15 (App Router)
- **Database**: PostgreSQL
- **ORM**: Drizzle ORM
- **Styling**: Tailwind CSS 4
- **Language**: TypeScript
- **Fonts**: Google Fonts (Inter, Playfair Display)

## 📦 Installation

### Prerequisites
- Node.js 18+
- PostgreSQL database

### Setup

1. **Clone the repository**
```bash
git clone https://github.com/YOUR_USERNAME/dr-manisha-health.git
cd dr-manisha-health
```

2. **Install dependencies**
```bash
npm install
```

3. **Set up environment variables**
```bash
cp .env.example .env
```
Edit `.env` with your database URL:
```
DATABASE_URL=postgresql://user:password@localhost:5432/dr_manisha_health
```

4. **Push database schema**
```bash
npx drizzle-kit push
```

5. **Seed the database** (optional)
```bash
npx tsx src/db/seed.ts
```

6. **Run development server**
```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to view the store.

## 🔐 Admin Access

Navigate to `/admin` and enter the password:
```
IRANIUMMARKO123
```

## 📁 Project Structure

```
src/
├── app/
│   ├── admin/           # Admin dashboard
│   ├── api/             # API routes
│   │   ├── admin/       # Admin CRUD APIs
│   │   ├── chat/        # Chat APIs
│   │   ├── products/    # Product APIs
│   │   └── ...
│   ├── checkout/        # Checkout flow
│   ├── products/        # Product pages
│   └── page.tsx         # Home page
├── components/
│   ├── ChatWidget.tsx   # Live chat
│   ├── Header.tsx       # Navigation
│   ├── Footer.tsx       # Footer
│   ├── ProductCard.tsx  # Product cards
│   ├── SlideOutCart.tsx # Cart drawer
│   └── ...
├── db/
│   ├── index.ts         # Database connection
│   ├── schema.ts        # Drizzle schema
│   └── seed.ts          # Seed data
└── lib/
    └── cart-context.tsx # Cart state management
```

## 🌐 Deployment

### Vercel (Recommended)
1. Push to GitHub
2. Import project in Vercel
3. Add `DATABASE_URL` environment variable
4. Deploy!

### Other Platforms
The app can be deployed to any platform supporting Node.js:
- Railway
- Render
- DigitalOcean App Platform
- AWS/GCP/Azure

## 📄 License

MIT License — feel free to use for personal or commercial projects.

## 🙏 Credits

- Stock images from [Pexels](https://pexels.com)
- Icons from Heroicons
- Fonts from Google Fonts

---

Built with ❤️ for seniors living their best lives.
