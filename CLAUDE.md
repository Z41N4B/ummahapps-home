# Ummah Apps home page

The home page for all the Ummah Apps, live at https://ummahapps.ai/

This file tells Claude (and anyone else working on the site) how the project works. It is part of the Ummah Apps family, listed at https://ummahapps.ai/.

## How this site works
- A plain static site: HTML, CSS and JavaScript with no build step and no server code. Most of the app is in `index.html`.
- It is hosted on GitHub Pages. Pushing to `main` puts it live within a minute or two. Keep the `CNAME` file, or the custom domain stops working.
- Nothing is uploaded. All progress is saved in the browser on the user's own device (localStorage, cookies or IndexedDB). There are no accounts, analytics or paid services.
- There is no README yet. `llms.txt` gives a short description of the site. If you add features, consider adding a README that explains them.

## Saved progress is precious
Learners may have months of progress saved on their devices. Never rename or remove a storage key, cookie or data field without code that moves the old data across. Old saved data must still load. When a data shape changes, test with data saved by the old version.

## Writing style
- Use plain, simple English everywhere: on screen, in the README and in commit messages. Many users are children, parents, or people whose first language isn't English.
- Commit messages are one short sentence saying what changed for the user, for example "Go to the next question by itself 2 seconds after a right answer".
- Keep Arabic fully vowelled (harakat) unless the app has a setting to hide the vowels.

## Religious content
- Never make up or paraphrase Qur'an text, hadith wording or duas. Use only wording that is already in the app or that the owner provides, and keep the source (for example the Sahih al-Bukhari or Sahih Muslim number on sunnah.com).
- Follow the Prophet's name with "peace be upon him" (or ﷺ).
- If unsure whether something is religiously correct, ask the owner instead of guessing.

## Search engines and AI tools (SEO and GEO)
When a feature, count or description changes, also update what describes it: the meta description, the JSON-LD and the FAQ in `index.html`, `llms.txt`, and the date in `sitemap.xml`.

## Before saying a change is done
- Run the site locally and check the change in the browser preview, including on a phone-sized screen.
- Check the browser console for errors.
- Ask the owner before committing or pushing, because pushing makes it live for everyone.

## Ummah Apps home page
- This is the front page at https://ummahapps.ai/, with a card for each app, grouped as Hifdh, Kids, Arabic, Family and Finance.
- When an app is added, renamed or removed, update its card here, plus `llms.txt` and the JSON-LD. Hisab (hisab.ummahapps.ai) is linked from here but its code is not in this folder.
- There is no README or `serve.js`. Run it locally with any static server from this folder, for example `npx serve .`
