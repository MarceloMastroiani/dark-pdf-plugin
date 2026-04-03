# Obsidian Dark PDF Plugin

A lightweight and high-performance plugin that automatically converts PDF viewing to Dark Mode within Obsidian. Designed for night-time researchers and vault-dwellers who prefer a consistent dark aesthetic.

---

## 🌙 Features

- **Automatic PDF Dark Mode**: Applies a readable dark theme to all PDFs opened in your vault.
- **Instant Toggle**: Use the command palette (`Toggle Dark PDF`) to switch between light and dark modes on the fly.
- **Eye-Friendly Filters**: Optimized CSS filters that invert colors while preserving readability and reducing eye strain.
- **Seamless Integration**: Works with Obsidian's native PDF viewer without third-party dependencies.

## 🚀 Installation

### Via BRAT (Recommended for Beta)
1. Install the [Obsidian42 - BRAT](https://github.com/TfTHacker/obsidian42-brat) plugin.
2. Go to **Settings** > **BRAT** > **Add Beta plugin**.
3. Paste the repository URL: `https://github.com/MarceloMastroiani/dark-pdf-plugin`.
4. Enable the plugin in **Community Plugins**.

### Manual Installation
1. Go to the [latest release](https://github.com/MarceloMastroiani/dark-pdf-plugin/releases) and download `main.js`, `manifest.json`, and `styles.css`.
2. Create a folder named `dark-pdf-plugin` inside your vault's `.obsidian/plugins/` directory.
3. Move the downloaded files into that folder.
4. Restart Obsidian or reload the plugin list, then enable it.

## 🛠 How to Use

Once the plugin is enabled:
1. Open any PDF file.
2. It will automatically apply the dark filter.
3. If you need to see the original colors (e.g., for complex diagrams), open the **Command Palette** (`Ctrl/Cmd + P`) and run `Dark PDF: Toggle Dark PDF`.

## 🎨 Customizing the Look

You can fine-tune the dark mode filter by adding a CSS snippet to Obsidian:

```css
/* Custom Dark PDF Filter */
.dark-pdf-mode .pdfViewer .page canvas,
.dark-pdf-mode .pdfViewer .page .textLayer {
  /* Try adjusting these values for your specific theme */
  filter: invert(0.9) hue-rotate(180deg) brightness(1.1) contrast(0.8) !important;
}
```

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/MarceloMastroiani/dark-pdf-plugin/issues).

## 📜 License

This project is [MIT](LICENSE) licensed.

---

*Made with ❤️ by [Marcelo Mastroiani](https://github.com/MarceloMastroiani)*
