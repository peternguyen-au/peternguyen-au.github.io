# Assets Directory

This directory contains static assets for the website.

## Adding Your PDF Resume

To add a downloadable PDF version of your resume:

1. Create or export your resume as a PDF file
2. Name it `resume.pdf`
3. Place it in this `/assets` directory
4. The download link is already set up on the main page

Alternatively, you can use any other filename and update the link in `index.md`:

```markdown
<a href="/assets/your-resume-name.pdf" class="pdf-link">📄 Download Resume</a>
```

## Other Assets

You can also place other files here such as:
- Images for blog posts (`/assets/images/`)
- Documents
- Other downloadable files

These can be referenced in your markdown files using:
```markdown
![Alt text](/assets/images/your-image.png)
[Download File](/assets/your-file.pdf)
```
