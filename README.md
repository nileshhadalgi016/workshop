# RoboWorkshop

Static site for robotics & electronics workshops (Arduino, Raspberry Pi, sensors, edge AI).

## Structure
`/index.html` landing page  
`/workshops.html` catalog with filter  
`/workshop.html?id=...` dynamic detail page (vanilla JS)  
`/tracks.html` learning paths  
`/about.html`, `contact.html`, `resources.html`  
`/assets/css` modular styles  
`/assets/js` data + rendering modules  

## Local Preview
Open `index.html` directly OR run a simple server:  

    python3 -m http.server 8000

Visit `http://localhost:8000`

## Adding a Workshop
Edit `assets/js/data.js` and append a new object to `workshops` array. Ensure unique `id`.

## Deploy (GitHub Pages)
1. Push to `main` branch.
2. In repository Settings > Pages: Source = `Deploy from a branch`, select `main` and `/ (root)`.
3. Save. Site URL: `https://<username>.github.io/workshop/`

## Custom Domain (optional)
Add `CNAME` file at repo root containing your domain (e.g. `robotworkshop.io`) then configure DNS CNAME to `<username>.github.io`.

## License
Proprietary (update if you choose OSS license).
