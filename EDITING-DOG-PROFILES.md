# Editing rescue profiles — simple guide

**You do not need Bark-Caster or a database to manage the website.** The dog listing is stored in `dogs.json` and photos in `assets/dogs/`.

## Change a dog's information
1. In your GitHub repository, open `dogs.json` and click the pencil (Edit) icon.
2. Find the dog's `"name"`. Update the relevant fields. Keep quotation marks, commas, brackets and JSON syntax intact.
3. Click **Commit changes**. GitHub Pages will republish the updated site.

Each dog uses these fields:
```json
{
  "name": "Example Dog",
  "status": "adoptable",
  "photo": "assets/dogs/example-dog.webp",
  "story": "A full approved public story about this dog."
}
```
- `status`: use `adoptable`, `sanctuary`, or `adopted`.
- `photo`: use the exact image filename in `assets/dogs/`; filenames are case-sensitive.
- `story`: preserve the approved wording. To insert a paragraph break in JSON, type `\n\n` inside the string.

## Add a new dog
1. Upload a photo to `assets/dogs/` in GitHub using **Add file → Upload files**.
2. Edit `dogs.json`, duplicate one existing dog object, and update name, status, photo path, and story.
3. Ensure objects are separated by commas and that the final object has no trailing comma.
4. Commit the change and refresh `dogs.html`.

## Remove a dog or mark adopted
- To keep their story visible as an alumni record, set `"status": "adopted"` (it appears when showing all dogs).
- To remove the dog entirely, delete that dog's whole object from the JSON list, ensuring the remaining commas are valid.
- Optionally remove the unused photo from `assets/dogs/` afterward.

## Check before committing
- Confirm the story and photo are approved for public release.
- Confirm the adoption status with the rescue.
- Make sure `dogs.json` is valid JSON. A missing comma or quote can prevent all profiles from loading.
- Check on a phone and a computer after GitHub Pages deploys.

## Troubleshooting
- **No profiles appear:** check `dogs.json` syntax and that the site is being served via GitHub Pages (opening `dogs.html` directly from a computer file folder can block JSON loading).
- **Missing photo:** check `photo` path and exact filename, including uppercase/lowercase.
- **Changes not visible:** wait for GitHub Pages deployment and refresh the page.

## Website files at a glance
- `index.html`: homepage
- `dogs.html`: dog profile listing (automatically reads `dogs.json`)
- `dogs.json`: edit all dog information here
- `assets/dogs/`: dog photos
- `styles.css`: design and mobile layout
- `script.js`: interactions and dog listing logic


All dog photos are now in the repository root (no assets folders). The `image` property in dogs.json should be the plain filename, such as `snow.webp`.
