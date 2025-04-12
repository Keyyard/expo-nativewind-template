# Expo NativeWind Template

This repository serves as a template for setting up an Expo project (SDK 50+) with NativeWind for styling. NativeWind is a library that brings Tailwind CSS to React Native, enabling utility-first styling in your mobile applications.

## Features

- **Expo SDK 50+**: Leverage the latest features of Expo.
- **NativeWind**: Use Tailwind CSS classes for styling in React Native.
- **Prettier Plugin for Tailwind CSS**: Automatically sort Tailwind classes for better readability.
- **TypeScript**: Strongly typed code for better developer experience.

## Prerequisites

- Node.js (v16 or later)
- npm or yarn
- Expo CLI

## Getting Started

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/expo-nativewind-template.git
   cd expo-nativewind-template
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```

3. Start the development server:
   ```bash
   npm start
   # or
   yarn start
   ```

4. Open the app on your device or emulator:
   - For Android: Press `a`
   - For iOS: Press `i`
   - For Web: Press `w`

## Project Structure

```
expo-nativewind-template/
├── assets/                # Static assets like images
├── components/            # Reusable React components
├── App.tsx                # Entry point of the application
├── global.css             # Tailwind CSS configuration
├── tailwind.config.js     # Tailwind CSS setup
├── metro.config.js        # Metro bundler configuration for NativeWind
├── tsconfig.json          # TypeScript configuration
├── package.json           # Project dependencies and scripts
└── README.md              # Project documentation
```

## Configuration

### Tailwind CSS
The `tailwind.config.js` file is pre-configured to work with NativeWind. You can extend the theme or add custom utilities as needed.

### Metro Bundler
The `metro.config.js` file is set up to include the `global.css` file for Tailwind CSS.

### Prettier
The `prettier.config.js` file includes the Tailwind CSS plugin to automatically sort classes.

## Adding New Components

1. Create a new file in the `components/` directory.
2. Use Tailwind CSS classes in the `className` attribute for styling.

Example:
```tsx
import { View, Text } from 'react-native';

export const MyComponent = () => {
  return (
    <View className="p-4 bg-blue-500">
      <Text className="text-white">Hello, NativeWind!</Text>
    </View>
  );
};
```

## References

- [NativeWind Documentation](https://github.com/nativewind/nativewind)
- [Expo Documentation](https://docs.expo.dev/)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)

## License
'
This project is licensed under the MIT License. See the LICENSE file for details.
