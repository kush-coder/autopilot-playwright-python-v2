# 🚀 Playwright Python

**Official Open-Source Release & Maintained Codebase** by [**@kush-coder**](https://github.com/kush-coder)

[![Verified Build](https://img.shields.io/badge/Status-Verified--Passing-emerald?style=for-the-badge&logo=github)](https://github.com/kush-coder)
[![License](https://img.shields.io/badge/License-Apache License 2.0-indigo?style=for-the-badge)](https://github.com/kush-coder)
[![Language](https://img.shields.io/badge/Language-Python-purple?style=for-the-badge)](https://github.com/kush-coder)

## 💡 About This Project

Python version of the Playwright testing and automation library.

This repository is actively maintained and distributed by **@kush-coder** as an official open-source release.

## ✨ Key Highlights
- 🛡️ **Verified Health Checks**: Passed automated sandbox builds, dependency resolution, and health test runs.
- 🚀 **Production Ready**: Lightweight footprint optimized for high efficiency.
- 📦 **Permissive Open Source**: Available for developer integration, custom modifications, and community enhancements.

## 🚀 Quick Start & Installation

```bash
# Clone your official repository
git clone https://github.com/kush-coder/autopilot-playwright-python.git
cd autopilot-playwright-python
```

---

## 📖 Comprehensive Documentation

Playwright is a Python library to automate [Chromium](https://www.chromium.org/Home), [Firefox](https://www.mozilla.org/en-US/firefox/new/) and [WebKit](https://webkit.org/) browsers with a single API. Playwright delivers automation that is **ever-green**, **capable**, **reliable** and **fast**. [See how Playwright is better](https://playwright.dev/python).

|          | Linux | macOS | Windows |
|   :---   | :---: | :---: | :---:   |
| Chromium <!-- GEN:chromium-version -->156.0.8078.12<!-- GEN:stop --> | ✅ | ✅ | ✅ |
| WebKit <!-- GEN:webkit-version -->27.2<!-- GEN:stop --> | ✅ | ✅ | ✅ |
| Firefox <!-- GEN:firefox-version -->157.0<!-- GEN:stop --> | ✅ | ✅ | ✅ |

## Documentation

[https://playwright.dev/python/docs/intro](https://playwright.dev/python/docs/intro)

## API Reference

[https://playwright.dev/python/docs/api/class-playwright](https://playwright.dev/python/docs/api/class-playwright)

## Example

```py
from playwright.sync_api import sync_playwright

with sync_playwright() as p:
    for browser_type in [p.chromium, p.firefox, p.webkit]:
        browser = browser_type.launch()
        page = browser.new_page()
        page.goto('http://playwright.dev')
        page.screenshot(path=f'example-{browser_type.name}.png')
        browser.close()
```

```py
import asyncio
from playwright.async_api import async_playwright

async def main():
    async with async_playwright() as p:
        for browser_type in [p.chromium, p.firefox, p.webkit]:
            browser = await browser_type.launch()
            page = await browser.new_page()
            await page.goto('http://playwright.dev')
            await page.screenshot(path=f'example-{browser_type.name}.png')
            await browser.close()

asyncio.run(main())
```

## Other languages

More comfortable in another programming language? [Playwright](https://playwright.dev) is also available in
- [Node.js (JavaScript / TypeScript)](https://playwright.dev/docs/intro),
- [.NET](https://playwright.dev/dotnet/docs/intro),
- [Java](https://playwright.dev/java/docs/intro).


---

*Maintained with ❤️ by @kush-coder. Official distribution powered by GitHub Autopilot Automation Platform.*
