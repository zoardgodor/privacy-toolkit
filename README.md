# 🔒 Privacy Toolkit

A curated, offline-ready directory of **150+ trustworthy privacy, security and anonymity tools**, organized into 23 categories. Built as a single self-contained static website — no build step, no external dependencies, no tracking.

---

## 📖 Project Description

**Privacy Toolkit** is a static website that catalogs real, existing, and legal privacy, security and anonymity resources — from encrypted email providers and VPN services to password managers, secure operating systems and security-testing utilities.

---

## 🗂️ Categories

| Category | Icon | Description |
|---|---|---|
| Account Cleanup | 🧹 | Tools to find and delete unused online accounts |
| Ad & Tracker Blocking | 🛡️ | Browser and network-level ad/tracker blockers |
| Anonymous Browsing | 🕵️ | Networks and tools for anonymous, censorship-resistant access |
| Browser Privacy Tests | 🔬 | Tests that reveal what your browser leaks |
| Data Breach Checkers | 🚨 | Services to check if your data has been exposed |
| DNS Privacy | 🌐 | Privacy-respecting DNS resolvers |
| Encrypted Cloud Storage | ☁️ | Zero-knowledge / end-to-end encrypted file storage |
| Encrypted Email | 📧 | End-to-end encrypted email providers |
| File Encryption | 🔐 | Local file and disk encryption software |
| Identity Protection | 🪪 | Identity theft monitoring and protection services |
| Metadata Tools | 🧾 | Tools to inspect and strip file metadata |
| Mobile Privacy | 📱 | Privacy-respecting Android tools and app stores |
| Open Source Privacy Projects | 🧩 | Open standards and foundational privacy projects |
| Password Managers | 🔑 | Secure password storage and generation |
| Privacy Guides | 📚 | Educational resources and best-practice guides |
| Privacy Search Engines | 🔎 | Search engines that don't track users |
| Privacy Tools | 🧰 | Email aliasing, virtual cards, and general privacy utilities |
| Privacy-focused Operating Systems | 💻 | Hardened desktop and mobile operating systems |
| Secure Browsers | 🌍 | Browsers built or configured for privacy |
| Secure Messaging | 💬 | End-to-end encrypted messaging apps |
| Security Testing | 🧪 | Network and web security auditing tools |
| Temporary Email | ✉️ | Disposable inbox services |
| VPN Services | 🛰️ | No-logs and privacy-respecting VPN providers |

Each category header displays a live count of the tools it contains.

---

## 🚀 How to Use

1. Open: https://zoardgodor.github.io/
2. Use the **search bar** at the top to instantly filter tools by name, description, or category.
3. Click a **category header** to expand or collapse it. Your collapsed/expanded state is saved locally in your browser.
4. Use the **Open ↗** button on any card to visit the tool's website, or **Copy URL** to copy the link to your clipboard.
5. Click the **↑ Back to top** button (appears after scrolling) to return to the top instantly.

---

## 🎨 Customization

Because everything lives in a single `index.html` file, customization is straightforward:

- **Add or edit tools**: locate the `TOOLS` array near the top of the `<script>` section and add an object in the form:
  ```js
  { cat:"Category Name", name:"Tool Name", url:"https://example.com/", desc:"Short description." }
  ```
- **Add a new category**: add an entry to the `CATEGORY_META` array with a `name` and an emoji `icon`, then add matching tools to `TOOLS` with the same `cat` value. Categories are rendered in the order defined in `CATEGORY_META`.
- **Change the color scheme**: all colors are defined as CSS custom properties inside `:root` at the top of the `<style>` block (e.g. `--accent`, `--bg`, `--surface`). Change these values to re-theme the entire site.
- **Adjust the card grid**: modify the `.category-body` `grid-template-columns` rule to change how many cards appear per row.
- **Disable persistence**: remove or modify the `localStorage` calls (`saveCollapsedState`) if you don't want collapsed-category state to be remembered between visits.

---

## 📄 License

This project is released under the **MIT License**.

```
MIT License

Copyright (c) 2026

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

**Disclaimer:** Links are provided for informational purposes. Always verify a tool's current reputation, jurisdiction, and audit history before relying on it for sensitive privacy or security needs.
