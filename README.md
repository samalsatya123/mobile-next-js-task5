# MaidMatch Mobile App

A mobile-first Next.js application that displays professional domestic helper profiles with pixel-perfect design implementation and seamless API integration.

## 🚀 Features

- **Next.js 13+ App Router**: Modern React framework with server-side rendering
- **TypeScript**: Fully typed with strict mode enabled
- **Tailwind CSS**: Utility-first styling with custom design system
- **Responsive Design**: Optimized for mobile viewports (375px, 390px, 430px)
- **API Integration**: Server-side data fetching with fallback handling
- **Performance Optimized**: Next.js Image optimization, dynamic imports, and Core Web Vitals optimization
- **SEO Friendly**: Dynamic metadata generation and semantic HTML structure
- **Accessibility**: WCAG compliant with proper focus management and ARIA labels

## 🛠 Tech Stack

- **Framework**: Next.js 14
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **UI Components**: Radix UI primitives
- **Image Optimization**: Next.js Image component
- **State Management**: React hooks with Radix UI Collapsible

## 📱 Design Implementation

### Pixel-Perfect Fidelity
The implementation achieves high fidelity to the original Figma design while making sensible improvements:

### Design Improvements Made:
1. **Enhanced Accessibility**: Added proper ARIA labels, focus management, and semantic HTML structure
2. **Improved Typography**: Consistent font loading and better text hierarchy
3. **Optimized Images**: Implemented Next.js Image component with proper alt text and lazy loading
4. **Responsive Enhancements**: Fluid design that works seamlessly across target viewport widths
5. **Interactive States**: Added hover effects and smooth transitions for better user experience
6. **Loading States**: Implemented skeleton loading for better perceived performance
7. **Error Handling**: Graceful error boundaries and fallback states

### Functional Features:
- **Expandable Accordions**: Fully functional expanded profile sections with smooth animations
- **Mobile Navigation**: Authentic mobile browser header simulation
- **Interactive Elements**: Hover states, focus indicators, and button interactions
- **Responsive Layout**: Adapts beautifully to different mobile screen sizes

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ 
- npm or yarn

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd maidmatch-mobile-app
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   ```bash
   cp .env.local.example .env.local
   ```
   Update the API endpoints in `.env.local` if needed.

4. **Run the development server**
   ```bash
   npm run dev
   ```

5. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

### Build for Production

```bash
npm run build
npm start
```

## 📁 Project Structure

```
src/
├── app/                    # Next.js App Router
│   ├── layout.tsx         # Root layout with metadata
│   ├── page.tsx           # Home page with SSR
│   ├── loading.tsx        # Loading UI
│   ├── error.tsx          # Error boundary
│   └── not-found.tsx      # 404 page
├── components/            # Reusable UI components
│   ├── ui/               # Base UI components (shadcn/ui)
│   ├── MobileHeader.tsx  # Mobile browser simulation
│   ├── ProfileHeader.tsx # Profile hero section
│   ├── ProfileSection.tsx # Main profile content
│   ├── InfoCard.tsx      # Reusable info display
│   ├── SkillGrid.tsx     # Skills display grid
│   ├── WorkExperienceList.tsx # Work history
│   ├── ExpectationsList.tsx   # Expectations display
│   ├── ExpandedProfile.tsx    # Collapsible sections
│   └── InterestButton.tsx     # CTA button
├── lib/                   # Utility functions
│   ├── api.ts            # API integration
│   └── utils.ts          # Helper functions
├── types/                 # TypeScript definitions
│   └── worker.ts         # API response types
└── styles/               # Global styles
    └── globals.css       # Tailwind and custom CSS
```

## 🔧 API Integration

The app integrates with the MaidMatch API to fetch worker profile data:

- **Endpoint**: `GET https://adminapi.maidmatch.ai/api/worker-detail/1058?type=document`
- **Method**: Server-side rendering with Next.js
- **Fallback**: Mock data for development and error scenarios
- **Caching**: 1-hour revalidation for optimal performance

### Type Safety
All API responses are strongly typed with comprehensive TypeScript interfaces, ensuring type safety throughout the application.

## 🎨 Styling Approach

- **Mobile-First**: Designed primarily for mobile with responsive enhancements
- **Custom Design System**: Tailwind configuration matches the original design tokens
- **Component-Based**: Reusable styled components for consistency
- **Performance**: Optimized CSS with Tailwind's purging and minimal runtime

## ⚡ Performance Optimizations

- **Image Optimization**: Next.js Image component with WebP/AVIF support
- **Code Splitting**: Dynamic imports for non-critical components
- **Server-Side Rendering**: Fast initial page loads with SEO benefits
- **Caching Strategy**: Appropriate cache headers and revalidation
- **Bundle Optimization**: Tree shaking and minimal JavaScript payload

## 🔍 SEO & Metadata

- **Dynamic Metadata**: Generated based on worker profile data
- **Open Graph**: Social media sharing optimization
- **Structured Data**: Semantic HTML with proper heading hierarchy
- **Meta Tags**: Comprehensive SEO tags including Twitter Cards

## 📱 Responsive Design

Optimized for three key mobile viewport widths:
- **375px**: iPhone SE, smaller Android phones
- **390px**: iPhone 12/13/14 standard models
- **430px**: iPhone 14 Pro Max, large Android phones

## 🧪 Development

### Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run lint` - Run ESLint
- `npm run type-check` - TypeScript type checking

### Code Quality

- **TypeScript**: Strict mode enabled for maximum type safety
- **ESLint**: Next.js recommended configuration
- **Prettier**: Consistent code formatting
- **Husky**: Pre-commit hooks for quality assurance

## 🚀 Deployment

The application is optimized for deployment on Vercel, Netlify, or any platform supporting Next.js:

1. **Build the application**
   ```bash
   npm run build
   ```

2. **Deploy to your preferred platform**
   - Vercel: `vercel deploy`
   - Netlify: Connect your repository
   - Docker: Use the included Dockerfile

## 📄 License

This project is part of a technical assessment and is not intended for commercial use.
And not disclose personal Information also like user name , password, and other details

---

Built with ❤️ using Next.js, TypeScript, and Tailwind CSS
