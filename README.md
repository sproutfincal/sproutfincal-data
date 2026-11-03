SproutFinCal Data & Web Resources

A centralized repository for hosting static HTML pages and JSON files used by SproutFinCal applications.

This repository uses GitHub Pages to make web pages and JSON resources publicly accessible over HTTPS, allowing applications to fetch and consume data directly.

🌐 GitHub Pages

Base URL:

https://sproutfincal.github.io/sproutfincal-data/

📁 Repository Structure
text
sproutfincal-data/
│
├── index.html
│
├── config/
│   └── app-config.json
│
├── data/
│   ├── categories.json
│   ├── settings.json
│   └── version.json
│
└── pages/
    └── example.html


The structure may evolve as new resources are added.

🚀 Usage
Access HTML Pages
text
https://sproutfincal.github.io/sproutfincal-data/pages/example.html

Fetch JSON Data

Applications can fetch JSON files directly using standard HTTP requests.

JavaScript example:

javascript
const response = await fetch(
  "https://sproutfincal.github.io/sproutfincal-data/data/categories.json"
);

const data = await response.json();

console.log(data);

🛠️ Technologies
HTML5
JSON
GitHub Pages
HTTPS
📝 Updates

Any changes pushed to the repository's published branch will be reflected on GitHub Pages after deployment.

🔒 Important Notes
All files published through GitHub Pages are publicly accessible.
Do not store API keys, passwords, private credentials, or sensitive user information.
Keep JSON files properly formatted and valid.
Maintain backward compatibility when updating JSON structures consumed by existing applications.
📄 License

Unless otherwise specified, the content in this repository is intended for use by SproutFinCal applications.
