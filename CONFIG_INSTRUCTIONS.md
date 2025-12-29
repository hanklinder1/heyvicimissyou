# 📝 How to Update Your Website

Everything is controlled by the `config.json` file! Just edit it to change your website.

## 🖼️ Changing Photos

1. **Add new photos**: Put image files in the `images/` folder
2. **Update config.json**: Edit the `photos` array:
   ```json
   "photos": [
     "images/your-photo-1.jpg",
     "images/your-photo-2.jpg"
   ]
   ```
3. **Single photo**: Just use one item in the array
4. **Multiple photos**: Add as many as you want - they'll display in a beautiful gallery!

## ✏️ Changing Text

- **Title**: Edit `"title"` 
- **Subtitle**: Edit `"subtitle"` (supports multiple lines with `\n`)
- **Note**: Edit `"note"` (your personal message)

## 🎵 Changing the Song

- **Spotify**: Paste any Spotify track URL
- **YouTube**: Paste any YouTube video URL
- **Remove music**: Delete the `"songUrl"` line or set it to `""`

## 💕 Adding Compliments

Edit the `"compliments"` array - add as many as you want! They'll be randomly shown when clicked.

## 🎯 Creating Quizzes

Edit the `"quiz"` object:
- `"question"`: Your question text
- `"options"`: Array of answer choices (add emojis for fun!)
- `"correctIndex"`: The correct answer (starts at 0, so first option = 0, second = 1, etc.)

## 📸 Adding Memories (Gallery Page)

Click "Memories" on the home page to see the full gallery! Add memories to the `"memories"` array:

```json
"memories": [
  {
    "photo": "images/photo1.jpg",
    "title": "Memory Title",
    "description": "A beautiful description of this special moment",
    "date": "2024"
  }
]
```

- **photo**: Path to the image (relative to website root)
- **title**: Title for this memory (optional)
- **description**: Description of the memory (optional)
- **date**: Date or year (optional)

You can add as many memories as you want! They'll display in a beautiful grid on the memories page.

## 🚀 After Making Changes

1. Save `config.json`
2. Commit and push to GitHub:
   ```bash
   git add config.json
   git commit -m "Updated website content"
   git push
   ```
3. Vercel will automatically deploy your changes!

## 💡 Tips

- Use emojis anywhere in text for extra personality! 😊
- Photos automatically resize and look great
- All sections are optional - remove them from config.json to hide them
- The website automatically adapts to mobile devices

