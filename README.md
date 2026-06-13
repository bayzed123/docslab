# SmartGen Documentation Hub

Welcome to the official documentation repository for **SmartGen** - an advanced QR code generation tool built by **Connect With Bayezid**. 

This repository serves as the central knowledge base, API reference, and user guide for SmartGen, powered by a fully automated GitOps architecture.

![Documentation Status](https://img.shields.io/badge/docs-live-brightgreen)
![Build Status](https://img.shields.io/badge/build-automated-blue)
![Framework](https://img.shields.io/badge/framework-MkDocs_Material-indigo)

## System Architecture

This documentation site is not a standard static HTML project. It uses a modern GitOps flow:
* **SSG Engine:** Built with [MkDocs Material](https://squidfunk.github.io/mkdocs-material/).
* **Zero-Touch Deployment:** Any push to the main branch automatically triggers a GitHub Actions workflow that builds the site and deploys it via Artifacts.
* **Dynamic Social Cards:** Automatically generates Open Graph images for seamless social media sharing.
* **Data Aggregation:** Includes custom Python scripts to fetch and aggregate guidelines from external repositories.

## Repository Structure

```text
docslab/
├── .github/workflows/      # CI/CD pipelines (GitHub Actions)
├── docs/                   # Markdown files containing the actual content
├── overrides/              # Custom HTML/CSS templates for MkDocs
├── layouts/                # Background images for dynamic social cards
├── scripts/                # Python scripts for external data aggregation
├── mkdocs.yml              # Main configuration file for the website
└── README.md               # You are reading this
```

## Local Development Setup

If you want to run this documentation site locally to preview changes before pushing them to the live server, follow these steps:

### Prerequisites
Make sure you have Python 3.8+ installed on your system. 

### Installation
1. **Clone the repository:**
```bash
   git clone [https://github.com/bayzed123/docslab.git](https://github.com/bayzed123/docslab.git)
   cd docslab
   ```

2. **Install the required dependencies:**
   *(Note: This includes MkDocs Material and libraries needed for social card generation)*
```bash
   pip install mkdocs-material pillow cairosvg
   ```

3. **Start the local live-reload server:**
```bash
   mkdocs serve
   ```
4. Open your browser and go to: http://127.0.0.1:8000

## How to Update the Docs

Updating the website is as simple as writing text. 
1. Navigate to the docs/ folder.
2. Edit or create a new .md (Markdown) file.
3. Commit and push your changes to the main branch.
4. The GitHub Actions bot will automatically build and publish the changes within seconds!

---

**Copyright Connect With Bayezid** | Managed by Sayad Md Bayezid Hosan
