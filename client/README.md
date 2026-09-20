# SEOnova

### AI-Powered SEO Analysis & Google Rank Tracking Platform

SEOnova is a full-stack AI-powered SEO platform that helps users analyze websites, identify SEO issues, receive AI-generated optimization recommendations, and track keyword rankings on Google over time.

The platform combines **browser automation, AI-powered analysis, REST APIs, MongoDB, and automated background jobs** to provide an end-to-end SEO monitoring solution.

---

## Features

### AI-Powered SEO Analysis

Analyze a website URL and generate a detailed SEO report containing:

- Overall SEO Score
- SEO Score
- Performance Score
- Accessibility Score
- Best Practices Score
- SEO Issues
- Issue Severity
- Optimization Recommendations
- Keyword Analysis

### Website Scraping

SEOnova uses **Playwright + Browserbase** to extract real website information including:

- Page Title
- Meta Description
- Canonical URL
- Robots Meta
- Open Graph Metadata
- Twitter Card Metadata
- Viewport
- Charset
- H1–H6 Headings
- Internal Links
- External Links
- Images
- Missing Image Alt Text
- Word Count
- Page Size
- Load Time
- HTTP Status

### Gemini AI Analysis

The extracted website data is passed to Gemini AI for analysis.

The AI evaluates the website and generates:

- SEO scores
- Keyword insights
- SEO issues
- Severity levels
- Optimization recommendations

### Google Keyword Rank Tracking

Track how a website ranks for specific keywords on Google.

The system:

- Scans up to 5 Google result pages
- Checks up to 50 search results
- Finds the target domain
- Stores the current ranking position
- Tracks position changes
- Stores ranking history
- Tracks the best ranking position
- Identifies competitors

### Automated Rank Updates

SEOnova uses `node-cron` to automatically update active keyword rankings.

The scheduled job runs:

```text
Every day at 6:00 AM
```
