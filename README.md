# ShoeCraftify 👟✨

> A next-generation shoe customization platform powered by AR/VR technology

## 📖 Overview

ShoeCraftify is an innovative web-based platform that revolutionizes the way users customize and purchase shoes. By combining cutting-edge AR/VR technology with intuitive design tools, we enable customers to visualize, customize, and perfect their dream shoes before making a purchase. Our platform integrates with leading footwear brands to provide an extensive catalog of styles and customization options.

## ✨ Features

### 🥽 AR/VR Try-On
- **Virtual Try-On**: Experience shoes in augmented reality before purchasing
- **360° View**: Rotate and examine shoes from every angle
- **Real-time Visualization**: See customizations instantly in AR/VR mode

### 🎨 Manual Customization
- **Color Palette**: Choose from a wide range of colors for different shoe components
- **Material Selection**: Pick from various materials and textures
- **Pattern & Stickers**: Add unique designs, patterns, and stickers
- **Text Customization**: Add personalized text and monograms

### 👔 Outfit Matching
- **Smart Recommendations**: AI-powered outfit suggestions based on your shoe design
- **Style Advisor**: Get fashion tips to complement your customized shoes
- **Virtual Wardrobe**: Match shoes with your existing wardrobe

### 🏢 Brand Integration
We've partnered with premium footwear brands:
- **Nike** - Athletic and lifestyle footwear
- **Adidas** - Sports and casual shoes
- **Woodland** - Outdoor and adventure footwear
- **RedTape** - Contemporary casual shoes
- **Craftman** - Artisan and premium leather shoes

### 🎯 Customization Zone
- **Color Customization**: Modify colors for sole, upper, laces, and accents
- **Shoe Types**: Choose from sneakers, boots, sandals, formal shoes, and more
- **Sticker Library**: Extensive collection of designs and graphics
- **Save & Share**: Save your designs and share with friends
- **Order History**: Track all your custom creations

## 🛠️ Technology Stack

### Frontend
- **React.js** - UI framework
- **Three.js** - 3D rendering and visualization
- **AR.js / WebXR** - Augmented reality features
- **Tailwind CSS** - Styling framework
- **Redux** - State management

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **MongoDB** - Database
- **Socket.io** - Real-time features

### AR/VR Technologies
- **WebGL** - 3D graphics rendering
- **A-Frame** - VR framework
- **Model Viewer** - 3D model display

### Additional Tools
- **Stripe** - Payment processing
- **AWS S3** - Asset storage
- **JWT** - Authentication

## 📦 Installation

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn
- MongoDB (local or cloud instance)

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/ayush2093/shoecraftify.git
   cd ShoeCraftify
   ```

2. **Install dependencies**
   ```bash
   # Install backend dependencies
   cd backend
   npm install
   
   # Install frontend dependencies
   cd ../frontend
   npm install
   ```

3. **Environment Configuration**
   
   Create a `.env` file in the `backend/` directory:
   ```env
   PORT=5001
   MONGODB_URI=mongodb://localhost:27017/shoecraftify
   SESSION_SECRET=your_session_secret
   FRONTEND_URL=http://localhost:5173
   NODE_ENV=development

   GOOGLE_CLIENT_ID=your_google_client_id
   GOOGLE_CLIENT_SECRET=your_google_client_secret
   CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
   CLOUDINARY_API_KEY=your_cloudinary_api_key
   CLOUDINARY_API_SECRET=your_cloudinary_api_secret
   EMAIL_USER=your_email@gmail.com
   EMAIL_PASSWORD=your_gmail_app_password
   RAZORPAY_KEY_ID=your_razorpay_key_id
   RAZORPAY_KEY_SECRET=your_razorpay_key_secret
   HF_TOKEN=your_huggingface_token
   ```

   Create a `.env` file in the `frontend/` directory:
   ```env
   VITE_APP_NAME=SHOECREATIFY
   VITE_BACKEND_URL=http://localhost:5001

   REACT_APP_CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
   REACT_APP_CLOUDINARY_PROFILE_PRESET=profile_pictures

   VITE_RAZORPAY_KEY_ID=your_razorpay_key_id
   RAZORPAY_KEY_SECRET=your_razorpay_key_secret
   RAZORPAY_STATIC_LINK=your_razorpay_payment_link
   ```

4. **Run the application**
   
   Run the backend dev server:
   ```bash
   cd backend
   npm run dev
   ```

   Run the frontend dev server:
   ```bash
   cd frontend
   npm run dev
   ```
   
5. **Access the application**
   - Frontend: http://localhost:5173
   - Backend API: http://localhost:5001

## 🚀 Usage Guide

### Getting Started

1. **Create an Account**
   - Sign up with email or social login
   - Complete your profile

2. **Browse Catalog**
   - Explore shoes from partnered brands
   - Filter by brand, type, size, and price

3. **Customize Your Shoe**
   - Select a base shoe model
   - Use the customization zone to modify:
     - Colors for different parts
     - Add stickers and patterns
     - Choose materials and finishes
   - Preview in 2D and 3D

4. **Try in AR/VR**
   - Enable camera access for AR mode
   - Use VR headset for immersive experience
   - Visualize shoes in your environment

5. **Outfit Matching**
   - Upload photos of your wardrobe
   - Get AI-powered outfit suggestions
   - Save favorite combinations

6. **Place Order**
   - Review your custom design
   - Select size and quantity
   - Complete secure checkout
   - Track your order

### Tips for Best Experience
- Use a device with camera for AR features
- Ensure good lighting for accurate AR visualization
- Save your designs to revisit later
- Share designs with friends for feedback

## 📁 Project Structure

```
ShoeCraftify/
├── backend/                # Backend Node.js Express server
│   ├── config/            # Transporter & Passport auth config
│   ├── models/            # Mongoose database models
│   ├── routes/            # Express router endpoints
│   ├── server.js          # Main entry file
│   └── package.json
├── frontend/               # Frontend React Vite application
│   ├── public/            # Static files & nikeShoes.glb 3D asset
│   ├── src/
│   │   ├── components/    # UI & editor views (Login, OTP, Payment)
│   │   ├── App.jsx        # Main application component
│   │   ├── main.jsx       # Client entry script
│   │   └── index.css      # Custom styling sheets
│   └── package.json
└── README.md             # Project documentation
```



<img width="962" height="649" alt="image" src="https://github.com/user-attachments/assets/9ad328f8-11ef-4055-adce-ed608a805467" />

## 🤝 Contributing

We welcome contributions from the community! Here's how you can help:

### How to Contribute

1. **Fork the repository**
   ```bash
   git clone https://github.com/ayush2093/shoecraftify
   ```

2. **Create a feature branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Make your changes**
   - Write clean, documented code
   - Follow existing code style
   - Add tests if applicable

4. **Commit your changes**
   ```bash
   git commit -m "Add: description of your feature"
   ```

5. **Push to your fork**
   ```bash
   git push origin feature/your-feature-name
   ```

6. **Open a Pull Request**
   - Provide a clear description of changes
   - Reference any related issues
   - Wait for review and feedback

### Contribution Guidelines

- **Code Quality**: Maintain high code quality and follow best practices
- **Documentation**: Update documentation for new features
- **Testing**: Include tests for new functionality
- **Commit Messages**: Use clear and descriptive commit messages
- **Issue First**: For major changes, open an issue first to discuss

### Areas for Contribution

- 🐛 Bug fixes
- ✨ New features
- 📝 Documentation improvements
- 🎨 UI/UX enhancements
- 🧪 Test coverage
- 🌐 Localization/translations
- ♿ Accessibility improvements

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### MIT License Summary

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software.

## 👥 Team

- **Project Lead**: Ayush Singh
- **GitHub**: (https://github.com/ayush2093)

## 🙏 Acknowledgments

- Thanks to all contributors who help improve ShoeCraftify
- Brand partners: Nike, Adidas, Woodland, RedTape, and Craftman
- Open-source community for amazing tools and libraries

## 🗺️ Roadmap

- [ ] Mobile app development (iOS/Android)
- [ ] AI-powered design recommendations
- [ ] Social sharing features
- [ ] Community design marketplace
- [ ] Advanced material simulation
- [ ] Integration with more brands
- [ ] Multi-language support

---

**Made with ❤️ by the ShoeCraftify Team**

*For diagram and architecture visualization, see [diagram.tldr](diagram.tldr)*
