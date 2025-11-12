# Website Customization Guide

## Current Setup

Your research paper website is now ready with:
- Complete paper details and abstract
- Key contributions section
- CLEAR methodology explanation
- Detailed findings and results
- Models evaluated
- Green AI implications
- BibTeX citation
- Links to arXiv and code repository

## Adding Figures/Images

To add figures from your paper:

1. **Extract images from PDF** or export from LaTeX
2. **Save images** to `static/images/` folder (e.g., `figure1.png`, `figure3.png`)
3. **Add to HTML** by inserting this code in the appropriate section:

```html
<div class="content has-text-centered">
  <img src="./static/images/figure1.png" alt="CLEAR Pipeline" style="max-width: 90%; height: auto;"/>
  <p class="has-text-centered"><strong>Figure 1:</strong> CLEAR pipeline overview</p>
</div>
```

### Recommended Figures to Add:

- **Figure 1**: CLEAR pipeline (after Methodology section)
- **Figure 3**: E/FLOP ratio comparison (in Results section)
- **Figure 4**: E/FLOP and ΔE/ΔFLOP analysis (in Results section)
- **Figure 6/7/8**: Energy breakdowns (in Results section)

## File Structure

```
research-paper-site/
├── index.html           # Main website file
├── static/
│   ├── paper.pdf       # Your paper PDF
│   ├── css/            # Stylesheets
│   ├── js/             # JavaScript files
│   └── images/         # Place your figures here
└── README.md
```

## Testing Locally

Open `index.html` in your browser to preview changes.

## Next Steps

1. Add figures to `static/images/`
2. Update `index.html` to reference the images
3. Test locally
4. Push to GitHub Pages
