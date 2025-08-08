# Files Directory

This directory is for storing static files (PDFs, images, documents) that are referenced throughout the site.

## Directory Structure

```
files/
├── pdfs/           # PDF documents (CV, papers, certificates)
├── images/         # Images for content pages
├── diagrams/       # Technical diagrams and flowcharts
└── downloads/      # Downloadable resources
```

## Usage

### Linking to files in markdown pages:

**For PDFs:**
```markdown
[Download my CV](files/pdfs/cv.pdf)
```

**For images:**
```markdown
![Project Screenshot](files/images/project-screenshot.png)
```

**For direct download links:**
```markdown
[Download Resource](files/downloads/resource.zip)
```

## File Naming Conventions

- Use lowercase letters
- Replace spaces with hyphens (-)
- Include dates where relevant (YYYY-MM-DD format)
- Keep names descriptive but concise

Examples:
- `cv-2024-01.pdf`
- `research-poster-aerospace-medicine.pdf`
- `project-screenshot-penny-finance.png`
- `diagram-system-architecture.svg`

## File Types

Recommended file types:
- **Documents**: PDF, DOCX (converted to PDF preferred)
- **Images**: PNG, JPG, SVG (for diagrams)
- **Data**: CSV, JSON
- **Archives**: ZIP

## Size Limits

Keep files reasonably sized for web delivery:
- PDFs: < 5MB
- Images: < 2MB (optimize for web)
- Downloads: < 10MB

For larger files, consider using external hosting and linking.

## Security Notes

- Don't store sensitive or private information
- Be careful with personally identifiable information
- Review files before committing to repository
- Remember this will be public on GitHub Pages