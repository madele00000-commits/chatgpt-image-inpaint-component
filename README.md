# ChatGPT Image Inpainting Component

A dependency-light, single-file browser demo for an image editing / inpainting workflow. The UI is implemented in `index.html` with Tailwind CSS CDN, Lucide icons, and HTML5 Canvas.

## Try it

Open `index.html` in a modern browser, or visit the GitHub repository and choose **Add file → Create new file** only if modifying. For a live preview, open the GitHub Pages URL after enabling Pages in repository Settings → Pages (Deploy from branch: `main`, folder `/ (root)`). You can also open the repository in github.dev with the `.` key and use a local preview extension, or download the file and open it directly.

## Features

- Local image upload and three remote sample photos
- Canvas-based pink mask brush with adjustable size, erase mode, and mask visibility
- Pointer Events for mouse, pen, and touch interactions
- Aspect ratio crop presets and PNG export
- Prompt entry and example prompt pills
- Responsive layout designed for desktop and mobile screens

## Important: generation backend

This is an interactive front-end demo, not a connected OpenAI/ChatGPT image-generation service. The Generate edit button intentionally reports that an API integration is needed; it does not fabricate generated results. To enable generation, implement a secure server-side endpoint for your chosen image model, send the source image plus a mask where required and the prompt, then render the returned image. Never expose a secret API key in browser JavaScript. External sample images require internet access; local uploads work offline.

## License

MIT. See `LICENSE`.
