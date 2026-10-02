# IMGLibOpen — New Complete Version

GitHub-only public image library. Firebase की जरूरत नहीं है।

## Repository setup
1. नया **Public** GitHub repository बनाइए।
2. ZIP की सभी files/folders `main` branch के root में रखें।
3. `Settings → Pages → Build and deployment → Deploy from a branch`
4. Branch `main`, Folder `/(root)` चुनकर Save करें।

`app.js` GitHub Pages URL से owner और repository name अपने-आप detect करता है।

## Structure
```text
index.html
styles.css
app.js
README.md
data/images.json
images/.gitkeep
```

## Password
Upload/Force password: `333784`

## Fine-grained token
केवल इसी repository के लिए Fine-grained PAT रखें और `Contents: Read and write` permission दें। Token को code/repository में publish न करें।

## Included features
- Mobile-first responsive UI
- Right-side Menu
- Upload
- Force Delete
- Normal/Dark mode
- All + Activity
- Search: image name, category, keywords, date
- Image Order: newest, oldest, name A–Z, name Z–A
- Multiple image upload
- Same category/keywords for a batch
- Multiple image Force Delete
- Same-page image viewer
- × close, outside-tap close, Escape close
- Download, Original, small 🗑 Force Delete
- Successful Force Delete के बाद image UI से तुरंत हटती है
- GitHub `data/images.json` metadata
- Diagnostic status when data fails
- No Firebase dependency

## Important
Browser password केवल gate है; असली repository authorization GitHub token से होता है। GitHub Pages repository public होना चाहिए ताकि public images दिखाई दें।

Image upload में practical GitHub API limits के कारण बहुत बड़ी files न रखें; इस version में 20 MB से बड़ी image browser से रोक दी जाती है।
