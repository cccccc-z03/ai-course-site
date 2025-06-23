# Video Hosting Setup Guide

## YouTube Setup (Recommended for beginners)

1. Upload video to YouTube
2. Copy video ID from URL: `https://youtube.com/watch?v=dQw4w9WgXcQ`
3. Replace in HTML:
```html
<iframe class="w-full h-full rounded-xl" 
        src="https://www.youtube.com/embed/dQw4w9WgXcQ" 
        frameborder="0" allowfullscreen></iframe>
```

## Vimeo Setup (Professional choice)

1. Upload to Vimeo
2. Get video ID from URL: `https://vimeo.com/123456789`
3. Replace in HTML:
```html
<iframe class="w-full h-full rounded-xl" 
        src="https://player.vimeo.com/video/123456789" 
        frameborder="0" allowfullscreen></iframe>
```

## Local Files (Small videos only)

1. Put video file in same folder as index.html
2. Reference directly:
```html
<video controls class="w-full h-full object-cover rounded-xl">
    <source src="./my-video.mp4" type="video/mp4">
</video>
```

## Deployment Platforms for Static Sites

### Netlify
- Drag & drop deployment
- Free tier: 100GB bandwidth/month
- Good for videos up to 100MB

### Vercel  
- GitHub integration
- Free tier: 100GB bandwidth/month
- Excellent performance

### GitHub Pages
- Free hosting
- Use with Git LFS for large files
- 1GB storage limit

### Firebase Hosting
- Google's platform
- Free tier: 1GB storage, 10GB transfer/month
- Easy setup with CLI 