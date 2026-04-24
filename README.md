# Gradient Generator

A simple, lightweight Gradient Generator built with HTML, CSS and JavaScript. Pick two colors, choose a direction, generate a CSS linear-gradient and copy the CSS to use in your projects.

![Gradient Generator preview](https://raw.githubusercontent.com/BinaryVortex/Gradient-Generator/main/Screenshot%202024-04-27%20153247.png)

## Demo (local)
1. Clone the repo:
   ```
   git clone https://github.com/BinaryVortex/Gradient-Generator.git
   ```
2. Open `index.html` in your browser:
   - Double-click the file or run: `open index.html` (macOS) / `xdg-open index.html` (Linux).

## Features
- Choose two colors using color pickers.
- Select gradient direction using intuitive arrow buttons (top, bottom, left, right, and diagonal).
- Generate the gradient and preview it live on the page background.
- Copy the CSS `background-image` value to clipboard with a single click.

## Example output
After choosing colors and direction, the generator produces a CSS rule like:
```css
background-image: linear-gradient(to bottom, #7986cb, #1a237e);
```

## How to use
1. Use the two color pickers to select your start and end colors.
2. Click one of the direction buttons to choose the gradient direction (the active button will be highlighted).
3. Click the "Generate" button to update the preview and populate the CSS in the output box.
4. Click "Copy" to copy the generated CSS to your clipboard and paste it into your stylesheet.

## Files
- `index.html` — HTML layout and UI structure.
- `style.css` — Styles for the panel and controls.
- `script.js` — JavaScript that handles direction selection, gradient generation, previewing, and copying.

Key functions in `script.js`:
- `setDirection(value, element)` — marks the clicked direction as active and updates the current direction.
- `generateCode()` — generates the `linear-gradient(...)` CSS and applies it to the page background.
- `copyText()` — selects the generated CSS text and copies it to the clipboard.

## Notes & credits
- Uses Font Awesome for icons and Google Fonts for typography (Rubik).
- Works offline — just open `index.html`.
- Filename note: the repository contains the screenshot as `Screenshot 2024-04-27 153247.png`; the README references the raw URL so GitHub will display it correctly.

## Contributing
Contributions are welcome! Open an issue or submit a pull request with improvements, features, or fixes.

## License
This project has no license file in the repository. If you want to apply a license, add a `LICENSE` file (for example MIT) or tell me which license you prefer and I can add one for you.
