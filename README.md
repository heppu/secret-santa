# Secret Santa 🎅🎄

A Christmas-themed web page to reveal your Secret Santa assignment with festive animations and falling snowflakes!

## Features

- 🎁 Beautiful Christmas-themed single-page application
- ❄️ Animated falling snowflakes
- 🎉 Gift box reveal animation
- 🔒 Secret Santa name passed as base64-encoded URL parameter
- 📱 Fully responsive design

## Usage

### Creating a Secret Santa Link

1. Encode the person's name in base64:
   ```bash
   # Using command line (Linux/Mac)
   echo -n "John Doe" | base64
   # Output: Sm9obiBEb2U=
   
   # Using JavaScript console
   btoa("John Doe")
   # Output: Sm9obiBEb2U=
   ```

2. Create the URL with the encoded name:
   ```
   index.html?name=Sm9obiBEb2U=
   ```

### Examples

- For "Santa Claus": `index.html?name=U2FudGEgQ2xhdXM=`
- For "Rudolph": `index.html?name=UnVkb2xwaA==`
- For "Mrs. Claus": `index.html?name=TXJzLiBDbGF1cw==`

### Running Locally

Simply open `index.html` in a web browser with the name parameter:

```bash
# Open in default browser (example for Linux)
xdg-open "index.html?name=Sm9obiBEb2U="

# Or for macOS
open "index.html?name=Sm9obiBEb2U="
```

### Deploying

Deploy the `index.html` file to any static web hosting service:
- GitHub Pages
- Netlify
- Vercel
- AWS S3
- Any web server

## How It Works

1. Open the page with a base64-encoded name parameter
2. See the animated Christmas gift box
3. Click the gift box to reveal your Secret Santa assignment
4. Enjoy the festive reveal animation! 🎉