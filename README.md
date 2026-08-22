# Sanskruti Samaj Seva Sansthan Trust Website

Official website for Sanskruti Samaj Seva Sansthan Trust, an NGO in Bharuch, Gujarat.

**Live Site:** https://sanskruti-samaj-sevatrust.github.io

## Running Locally

To run the website locally, use a live server. The site requires a server due to CORS restrictions when loading components dynamically.

Using Python 3:
```bash
python -m http.server 8000
```

Then open your browser and navigate to `http://localhost:8000`

## Image Loading

Images are loaded sequentially by number. Place images in their respective folders in `/images/` with sequential naming:

- `1.webp`
- `2.webp`
- `3.webp`
- etc.

The JavaScript automatically discovers and loads images in order. When a numbered file is not found, the slider stops searching and begins rotation.

## GitHub Action - WebP Conversion

A GitHub Action automatically converts uploaded images to WebP format. When you push images to the repository, the action:

1. Detects new image files
2. Converts them to WebP format
3. Commits the converted files back to the repository

This ensures all images are optimized and in the modern WebP format for better performance.
