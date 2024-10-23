# md-ui

**md-ui** is a Material Design 3 component library built with Pigment CSS for use in React and Next.js applications. The library aims to provide a set of customizable and accessible UI components that adhere to Material Design guidelines, making it easier for developers to build beautiful and functional user interfaces.

## Features

- **Material Design 3 Compliance**: Components are designed according to the latest Material Design guidelines.
- **Customizable Themes**: Easily switch between themes to fit your application's branding.
- **Accessible Components**: Built with accessibility in mind, ensuring all components are usable for all users.
- **Lightweight**: Utilizes Pigment CSS for minimalistic styles without sacrificing performance.
- **React & Next.js Support**: Fully compatible with React and Next.js frameworks.

## Installation

To install **MD-UI**, you can use npm:

```bash
npm install @pigment-css/react
npm install --save-dev @pigment-css/nextjs-plugin
```

### Next.js Setup

To integrate Pigment CSS with your Next.js project, update your `next.config.js` as follows:

```javascript
// next.config.js
const { withPigment } = require('@pigment-css/nextjs-plugin');

module.exports = withPigment({
  reactStrictMode: true,
});
```

## Usage

### Importing Components

You can import and use the components in your application as shown below:

```tsx
import { Button } from 'md-ui';

function App() {
  return (
    <div>
      <Button label="Click Me" onClick={() => alert('Button clicked!')} />
    </div>
  );
}
```

### Example

Here's an example of how to use **MD-UI** components in a Next.js page:

```tsx
// src/app/page.tsx
import { Button } from 'md-ui';

export default function Home() {
  const handleClick = () => {
    alert('Button clicked!');
  };

  return (
    <div>
      <h1>Welcome to MD-UI</h1>
      <Button label="Click Me" onClick={handleClick} />
    </div>
  );
}
```

## Documentation

For detailed documentation on each component and its props, please refer to the [Documentation](./docs).

## Contributing

Contributions are welcome! If you'd like to contribute to **MD-UI**, please fork the repository and create a pull request. Ensure your code adheres to the project's coding standards.

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.

## Acknowledgments

- [Pigment CSS](https://pigmentcss.com) for providing a powerful styling framework.
- [Material Design](https://material.io/design) for guidelines and inspiration.
