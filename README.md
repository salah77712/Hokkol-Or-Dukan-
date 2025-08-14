# হক্কল অর দোকান | Hokkol Or Dukan

An AI-powered agricultural marketplace platform that connects farmers directly with buyers, enabling fresh produce sales with modern technology integration.

## 🌾 Project Overview

**Hokkol Or Dukan** is a comprehensive agricultural marketplace designed to bridge the gap between farmers and consumers in Bangladesh. The platform provides a modern, user-friendly interface for buying and selling fresh produce while supporting local agriculture.

### Key Features

- **Dual User Interfaces**: Separate experiences for buyers and farmers
- **Bilingual Support**: English and Bengali (বাংলা) language support
- **Authentication System**: Email/password and phone OTP authentication
- **Product Management**: Comprehensive product catalog with categories
- **Real-time Updates**: Live inventory and order status updates
- **Image Storage**: Integrated file upload for product images
- **Location-based Filtering**: District-wise product discovery
- **Review System**: Product and farmer rating system
- **Shopping Cart & Orders**: Complete e-commerce functionality

## 🛠️ Technology Stack

### Frontend
- **React 18** with functional components and hooks
- **Vite** for fast development and building
- **TailwindCSS** for modern, responsive design
- **Framer Motion** for smooth animations
- **React Router Dom** for navigation
- **Lucide React** for icons

### Backend & Database
- **Supabase** for backend services
- **PostgreSQL** database with Row Level Security
- **Real-time subscriptions** for live updates
- **File storage** for images and documents

### State Management
- **React Context** for authentication
- **Custom hooks** for data fetching
- **Service layer** for API interactions

## 📦 Installation

### Prerequisites
- Node.js 18 or higher
- npm or yarn package manager
- Supabase account and project

### Setup

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd hokkol-or-dukan
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Environment Configuration**
   Create a `.env` file in the root directory:
   ```env
   VITE_SUPABASE_URL=your_supabase_project_url
   VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
   ```

4. **Database Setup**
   - Run the migration file in your Supabase SQL editor:
   ```sql
   -- Execute supabase/migrations/20250813094758_hokkol_or_dukan_marketplace.sql
   ```

5. **Start the development server**
   ```bash
   npm start
   ```

The application will be available at `http://localhost:5173`

## 🗃️ Database Schema

### Core Tables
- **user_profiles**: User information and preferences
- **products**: Product catalog with multilingual support
- **categories**: Product categories
- **districts**: Geographic location data
- **farmer_profiles**: Extended farmer information
- **orders & order_items**: Order management
- **cart_items**: Shopping cart functionality
- **reviews**: Product and farmer reviews
- **wishlists**: User wishlist functionality

### Storage Buckets
- **product-images**: Public product images (5MB limit)
- **user-avatars**: User profile pictures (2MB limit)

## 🔐 Authentication & Security

- **Row Level Security (RLS)** enabled on all tables
- **User-based access control** for data isolation
- **Secure file storage** with proper access policies
- **Role-based permissions** (buyer, farmer, admin)

## 🌍 Internationalization

The application supports:
- **English (en)**: Default language
- **Bengali (বাংলা)**: Native language support
- **Dynamic language switching**
- **Localized content** for product names and descriptions

## 🚀 Key Features Implementation

### For Buyers
- Browse products with advanced filtering
- District-based product discovery
- Shopping cart and checkout process
- Order tracking and history
- Farmer profiles and reviews
- Wishlist functionality

### For Farmers
- Product management dashboard
- Order management and fulfillment
- Profile customization with farm details
- Sales analytics and statistics
- Customer communication tools

### Admin Features
- User management
- Content moderation
- System analytics
- Category and district management

## 📱 Responsive Design

The application is fully responsive with:
- **Mobile-first approach**
- **Adaptive navigation** for different screen sizes
- **Touch-optimized interactions**
- **Progressive Web App (PWA) ready**

## 🧪 Demo Data

The application includes comprehensive demo data:
- **Sample farmers** with verified profiles
- **Product catalog** across multiple categories
- **Demo user accounts** for testing
- **Order samples** showing complete workflows

### Demo Credentials
- **Farmer**: farmer1@example.com / farmer123
- **Buyer**: buyer1@example.com / buyer123
- **Phone**: +8801700000000 / OTP: 1234

## 🔧 Development

### Project Structure
```
src/
├── components/        # Reusable UI components
├── contexts/         # React contexts (Auth, etc.)
├── pages/           # Page components
├── services/        # API service layers
├── lib/             # Utility libraries
├── utils/           # Helper functions
└── styles/          # Global styles
```

### Key Services
- **productService**: Product CRUD operations
- **cartService**: Shopping cart management
- **orderService**: Order processing
- **farmerService**: Farmer profile management
- **storageService**: File upload/management

## 🚀 Deployment

The application is ready for deployment on:
- **Vercel** (recommended for React apps)
- **Netlify**
- **Firebase Hosting**
- **Any static hosting service**

Make sure to:
1. Set environment variables in your hosting platform
2. Ensure Supabase project is properly configured
3. Test all authentication flows post-deployment

## 🤝 Contributing

Contributions are welcome! Please:
1. Fork the repository
2. Create a feature branch
3. Follow the existing code style
4. Add tests if applicable
5. Submit a pull request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🆘 Support

For support and questions:
- Create an issue in the repository
- Check existing documentation
- Review demo data and examples

## 🎯 Future Enhancements

Planned features include:
- **Payment Gateway Integration** (bKash, Nagad, SSLCommerz)
- **Delivery Tracking** with GPS integration
- **Advanced Analytics** for farmers and admins
- **Mobile Application** (React Native)
- **AI-powered recommendations**
- **Inventory management** tools
- **Multi-vendor marketplace** features

---

**Built with ❤️ for the farming community of Bangladesh**