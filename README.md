# 🍳 Recipe App Frontend

A modern, feature-rich React Native recipe application built with Expo, offering seamless recipe discovery, favorites management, and user authentication.

## ✨ Features

- 🔍 **Smart Recipe Search** - Find recipes with real-time search and debounced queries
- 📱 **Category Filtering** - Browse recipes by categories with intuitive filters
- ❤️ **Favorites Management** - Save and organize your favorite recipes
- 🔐 **User Authentication** - Secure sign-up, sign-in, and email verification
- 📖 **Detailed Recipe View** - Complete recipe information with ingredients and instructions
- 🎨 **Modern UI/UX** - Clean, responsive design with smooth animations
- 🌙 **Optimized Performance** - Efficient loading states and error handling

## 🚀 Tech Stack

### **Frontend Framework**
- **React Native** with **Expo** - Cross-platform mobile development
- **Expo Router** - File-based navigation system

### **Core Libraries**
- **React Hooks** - Modern state management and lifecycle handling
- **Custom Hooks** - Reusable logic with `useDebounce` for search optimization

### **UI & Styling**
- **StyleSheet API** - Modular styling architecture
- **Custom Components** - Reusable UI components
- **Responsive Design** - Adaptive layouts for different screen sizes

### **API Integration**
- **Fetch API** - HTTP client for external API calls
- **TheMealDB API** - Recipe data source
- **Custom API Service** - Centralized API management

### **Development Tools**
- **ESLint** - Code linting and formatting
- **TypeScript Configuration** - Type safety setup
- **Git** - Version control



## 🛠️ Installation & Setup

### Prerequisites
- **Node.js** (v16 or higher)
- **npm** or **yarn**
- **Expo CLI** (`npm install -g @expo/cli`)
- **iOS Simulator** (for iOS development) or **Android Studio** (for Android)

### Quick Start

1. **Clone the repository**

   git clone <repository-url>
   cd recipe-app-frontend


2. **Install dependencies**

   npm install
   # or
   yarn install


3. **Start the development server**

   npx expo start


4. **Run on device/simulator**
   - Press `i` for iOS simulator
   - Press `a` for Android emulator
   - Scan QR code with Expo Go app on your device

## 🔧 Configuration

### Environment Setup
Create a `.env` file in the root directory:


## 📱 App Screens

### 🏠 Home Screen (`app/(tabs)/index.jsx`)
- Featured recipes display
- Category-based browsing
- Quick access to popular recipes

### 🔍 Search Screen (`app/(tabs)/search.jsx`)
- Real-time recipe search with debouncing
- Category filtering
- Search results with recipe cards

### ❤️ Favorites Screen (`app/(tabs)/favorites.jsx`)
- User's saved favorite recipes
- Easy management of favorites
- Empty state handling

### 📖 Recipe Detail Screen (`app/recipe/[id].jsx`)
- Complete recipe information
- Ingredients list
- Step-by-step instructions
- Add/remove from favorites

### 🔐 Authentication Screens (`app/(auth)/`)
- **Sign In**: User login with validation
- **Sign Up**: New user registration
- **Email Verification**: Account verification flow

## 🎨 Key Components

### `RecipeCard.jsx`
Reusable recipe card component with:
- Recipe image and title
- Category and area information
- Favorite toggle functionality
- Navigation to recipe details

### `CategoryFilter.jsx`
Dynamic category filtering with:
- Horizontal scrollable categories
- Active state management
- Smooth selection animations

### `LoadingSpinner.jsx`
Consistent loading states across the app

### `SafeScreen.jsx`
Safe area wrapper for consistent screen layouts

## 🔗 Custom Hooks

### `useDebounce.js`
Optimizes search performance by debouncing user input:

const debouncedSearchTerm = useDebounce(searchTerm, 500);


## 🎯 Performance Optimizations

- **Debounced Search** - Reduces API calls during typing
- **Image Lazy Loading** - Optimized image rendering
- **Component Memoization** - Prevents unnecessary re-renders
- **Efficient State Management** - Minimal state updates
- **Error Boundaries** - Graceful error handling

## 🚀 Build & Deployment

### Development Build

npx expo start --dev-client


### Production Build

# For iOS
npx expo build:ios

# For Android
npx expo build:android

# Using EAS Build (recommended)
npx eas build --platform all


### Publishing Updates

npx expo publish


## 🧪 Testing


# Run tests
npm test

# Run with coverage
npm run test:coverage

# Run linting
npm run lint


## 📄 Scripts


{
  "start": "expo start",
  "android": "expo start --android",
  "ios": "expo start --ios",
  "web": "expo start --web",
  "build": "expo build",
  "lint": "eslint .",
  "test": "jest"
}


## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


## 🙏 Acknowledgments

- **TheMealDB** - For providing the comprehensive recipe API
- **Expo Team** - For the amazing development platform
- **React Native Community** - For continuous support and resources

## 📞 Support

For support, email your-navneet3771@gmail.com or create an issue in the repository.

---

**Made with ❤️ using React Native & Expo**