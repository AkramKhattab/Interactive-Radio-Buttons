# Interactive Radio Buttons

A lightweight JavaScript library that transforms traditional radio buttons into interactive, animated elements with customizable styles and smooth transitions.

![License](https://img.shields.io/badge/license-MIT-blue.svg)

## Features

- 🎨 Fully customizable styles and animations
- 🚀 Zero dependencies
- 📱 Responsive and mobile-friendly
- ⚡️ Lightweight (~2KB minified)
- 🔌 Easy integration with existing forms
- 🎭 Multiple themes available

## Demo

Check out the [live demo](https://akramkhattab.github.io/Interactive-Radio-Buttons/) to see Interactive Radio Buttons in action.

## Installation

### Using NPM

```bash
npm install interactive-radio-buttons
```

### Using CDN

Add the following lines to your HTML:

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/akramkhattab/Interactive-Radio-Buttons/dist/style.css">
<script src="https://cdn.jsdelivr.net/gh/akramkhattab/Interactive-Radio-Buttons/dist/interactive-radio.min.js"></script>
```

## Usage

1. Add the HTML structure:

```html
<div class="radio-group">
    <input type="radio" id="option1" name="options" value="1">
    <label for="option1">Option 1</label>
    
    <input type="radio" id="option2" name="options" value="2">
    <label for="option2">Option 2</label>
</div>
```

2. Initialize the Interactive Radio Buttons:

```javascript
const radioGroup = new InteractiveRadio('.radio-group');
```

## Customization

You can customize the appearance using CSS variables:

```css
:root {
    --radio-color: #007bff;
    --radio-size: 20px;
    --animation-duration: 0.3s;
}
```

## API Reference

### Constructor

```javascript
new InteractiveRadio(selector, options)
```

#### Parameters:

- `selector`: String or DOM Element
- `options`: Object (optional)
  - `animationDuration`: Number (default: 300)
  - `theme`: String (default: 'default')
  - `onChange`: Function

### Methods

- `getValue()`: Returns the current selected value
- `setValue(value)`: Sets the selected value
- `disable()`: Disables the radio group
- `enable()`: Enables the radio group

## Events

```javascript
radioGroup.on('change', (value) => {
    console.log('Selected value:', value);
});
```

## Browser Support

- Chrome 49+
- Firefox 52+
- Safari 10+
- Edge 16+
- Opera 36+

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

Josh Dillon
 - [CodePen Profile](https://codepen.io/jdillon/pens/public)
