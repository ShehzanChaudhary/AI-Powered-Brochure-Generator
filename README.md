## 🚀 AI-Powered Brochure Generator

An intelligent AI-based system that automatically scrapes, understands, and generates brochures from company websites.
This project combines web scraping + content processing + AI generation to create structured, readable, and visually appealing brochures.

## 📌 Overview

The AI-powered brochure generator takes a company website as input and:

1. Scrapes relevant website content
2. Extracts important information (about, services, products, etc.)
3. Navigates internal links intelligently
4. Uses AI to generate a clean, structured brochure

This eliminates manual effort in creating company profiles or marketing materials.

## ⚙️ Features
- 🌐 Intelligent website scraping
- 🔗 Automatic link discovery and navigation
- 🧹 Content cleaning (removes scripts, images, unnecessary tags)
- 🤖 AI-generated brochure content
- 📄 Structured output (ready for PDF / presentation use)
- ⚡ Fast and lightweight

## 🏗️ Project Structure
- ├── scraper.py              # Handles website scraping and link extraction
- ├── BrochureGenerator.ipynb # Main logic and AI generation workflow
- ├── README.md              # Project documentation
  
## 🧠 How It Works
1. Website Scraping

The system fetches website content using requests and parses it using BeautifulSoup.

Example:

Extracts page title
Cleans body content
Removes unnecessary elements like scripts, styles, images

👉 Implemented in: scraper.py

2. Link Extraction
Collects all internal links from the webpage
Helps in navigating deeper into the website
Enables multi-page understanding of the company
3. Content Processing
Filters relevant text
Truncates content for efficiency
Prepares structured input for AI
4. AI Brochure Generation
Uses processed content
Generates:
Company overview
Services
Key highlights
Structured brochure format

## 🛠️ Tech Stack
Python
BeautifulSoup – HTML parsing
Requests – Web scraping
Jupyter Notebook – Development & experimentation
AI Model (LLM) – Content generation

## 📦 Installation
git clone https://github.com/ShehzanChaudhary/AI-Powered-Brochure-Generator.git
cd ai-brochure-generator
Run Notebook

## ▶️ Usage
Step 1: Run Scraper
from scraper import fetch_website_contents, fetch_website_links

url = "https://example.com"

content = fetch_website_contents(url)
links = fetch_website_links(url)

Step 2: Generate Brochure
Open BrochureGenerator.ipynb
Provide:
Website content
Extracted links
Run cells to generate brochure

## 📄 Example Output
Company Name: XYZ Tech

About:
XYZ Tech is a leading company in...

Services:
- AI Solutions
- Cloud Computing
- Data Analytics

Highlights:
- Innovative technology
- Global presence
  
## 🚧 Future Improvements
- 🔍 Smarter link prioritization (only important pages)
- 🧠 Better AI summarization
- 🎨 Direct PDF/Design export
- 🌍 Multi-language support
- ⚡ Async scraping for speed
