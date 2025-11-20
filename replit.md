# Live News App - React Capstone Project

A comprehensive, production-ready news application built with React, TypeScript, and Express. Features real-time news from NewsAPI with beautiful UI, dark mode, responsive design, and seamless navigation.

## 🚀 Features

### Core Functionality
- **Top Headlines**: Curated breaking news on homepage with featured article layout
- **Category Browse**: 6 news categories - Technology, Business, Sports, Entertainment, Health, Science
- **Search**: Full-text search across all news articles with real-time results
- **Responsive Design**: Mobile-first approach with perfect tablet and desktop layouts
- **Dark/Light Mode**: Elegant theme toggle with localStorage persistence

### Technical Highlights
- **React + TypeScript**: Fully typed codebase for reliability and maintainability
- **React Query**: Efficient data fetching with caching and error handling
- **Wouter**: Lightweight SPA routing for seamless navigation
- **NewsAPI Integration**: Real news from 150,000+ sources worldwide
- **Shadcn UI**: Beautiful, accessible component library with Tailwind CSS
- **Loading States**: Skeleton loaders for optimal perceived performance
- **Error Handling**: Graceful error states with retry functionality

## 📁 Project Structure

```
├── client/
│   ├── src/
│   │   ├── components/          # Reusable UI components
│   │   │   ├── ThemeProvider.tsx    # Dark/light mode context
│   │   │   ├── Navbar.tsx           # Navigation with search
│   │   │   ├── NewsCard.tsx         # Article display card
│   │   │   ├── NewsLoader.tsx       # Skeleton loading state
│   │   │   ├── ErrorState.tsx       # Error display
│   │   │   └── EmptyState.tsx       # No results state
│   │   ├── pages/               # Route components
│   │   │   ├── HomePage.tsx         # Top headlines
│   │   │   ├── CategoryPage.tsx     # Category news
│   │   │   └── SearchPage.tsx       # Search results
│   │   ├── lib/                 # Utilities
│   │   │   └── queryClient.ts       # React Query setup
│   │   ├── App.tsx              # Root component with routing
│   │   └── index.css            # Global styles
│   └── index.html               # HTML entry point
├── server/
│   ├── routes.ts                # API endpoints
│   └── index.ts                 # Express server
└── shared/
    └── schema.ts                # Shared TypeScript types
```

## 🛠️ Technologies Used

### Frontend
- **React 18**: Modern hooks-based architecture
- **TypeScript**: Type safety and IntelliSense
- **Wouter**: SPA routing (4KB alternative to React Router)
- **React Query**: Server state management
- **Tailwind CSS**: Utility-first styling
- **Shadcn/ui**: High-quality component library
- **Lucide Icons**: Beautiful icon set
- **date-fns**: Date formatting utilities

### Backend
- **Express**: Web server framework
- **NewsAPI**: News data provider
- **Zod**: Runtime schema validation

## 🎨 Design System

### Colors
- **Primary**: Blue accent (#2563EB)
- **Background**: White (light) / Dark gray (dark)
- **Cards**: Subtle elevation with hover effects
- **Text**: Three-level hierarchy for readability

### Typography
- **Headings**: Inter (sans-serif) - clean, modern
- **Body**: Merriweather (serif) - readable, elegant
- **Sizes**: Responsive scale from mobile to desktop

### Components
- **Navbar**: Fixed top, blur background, responsive menu
- **NewsCard**: Image, title, description, metadata, CTA
- **Buttons**: Multiple variants (default, outline, ghost)
- **Loading**: Animated skeleton matching card layout

## 🔧 Setup & Configuration

### Prerequisites
- Node.js 20+
- NewsAPI key (free from https://newsapi.org/register)

### Environment Variables
```
NEWS_API_KEY=your_api_key_here
SESSION_SECRET=your_session_secret
```

### Installation
```bash
npm install
npm run dev
```

## 📱 Responsive Breakpoints

- **Mobile**: < 768px
  - Hamburger menu
  - Single column grid
  - Expandable search
  
- **Tablet**: 768px - 1024px
  - 2-column article grid
  - Partial category navigation
  
- **Desktop**: > 1024px
  - 3-column article grid
  - Full navigation bar
  - Featured article takes 2 columns

## 🌐 API Routes

### GET `/api/news/top-headlines`
Returns top news headlines for homepage
- **Response**: NewsApiResponse with articles array

### GET `/api/news/category/:category`
Returns news for specific category
- **Params**: category (technology|business|sports|entertainment|health|science)
- **Response**: NewsApiResponse with filtered articles

### GET `/api/news/search?q=query`
Searches news articles
- **Query**: q (search term)
- **Response**: NewsApiResponse with matching articles

## 🎯 Key Features Explained

### Theme Toggle
- Context-based theme management
- Persists to localStorage
- Smooth transitions between modes
- Respects system preference as default

### Category Navigation
- SPA navigation with wouter
- Active state highlighting
- Mobile-friendly drawer menu
- SEO-friendly URLs

### Search Functionality
- Real-time search as you type
- URL-based search state
- Results count display
- Empty state handling

### Loading States
- Skeleton loaders match actual content
- Prevent layout shift
- Smooth fade-in transitions
- Optimistic UI updates

### Error Handling
- Graceful API error display
- Retry functionality
- Clear error messages
- Fallback states

## 🏆 Capstone Project Requirements Met

✅ React + Fetch API (via React Query wrapper)  
✅ Navbar with 6 categories  
✅ Search bar with submission  
✅ Category-based news fetching  
✅ Search results display  
✅ News cards with image, title, description, source, date, "Read More"  
✅ useState and useEffect for state management  
✅ Loading skeleton UI  
✅ Error handling  
✅ Fully responsive (Grid/Flex)  
✅ Light/Dark mode toggle  
✅ Clean component structure  
✅ Separate components (Navbar, NewsCard, Loader, CategoryPage)  
✅ React Router (wouter) navigation  

## 🚀 Deployment

The app is ready for deployment on Replit. Simply click "Publish" to make it live with a custom .replit.app domain.

## 📝 Future Enhancements

- [ ] Pagination or infinite scroll
- [ ] Article bookmarking
- [ ] Advanced filters (date, source, language)
- [ ] Social sharing
- [ ] PWA support
- [ ] Article preview modal
- [ ] Reading list

## 👨‍💻 Development Notes

### Code Quality
- Fully typed with TypeScript
- Consistent component patterns
- Reusable utility functions
- Clean separation of concerns

### Performance
- React Query caching
- Lazy image loading
- Optimized re-renders
- Bundle size optimization

### Accessibility
- Semantic HTML
- ARIA labels
- Keyboard navigation
- Screen reader friendly

## 📄 License

This is a capstone educational project. NewsAPI data is subject to their terms of service.

---

**Built with ❤️ using React, TypeScript, and modern web technologies**
