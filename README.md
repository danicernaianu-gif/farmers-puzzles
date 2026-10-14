# The Farmer's Puzzles · Hawkstone

Three daily farm puzzles (Stook, Headland, Rotation) plus the bonus round, On the Edge. The whole thing is one file, `index.html`, so there is nothing to build or install.

## Two versions

When the page opens (after the 18+ check), people pick one:

- **Weekly.** What a player will see. The whole week is open, every game has unlimited hints and a Reset button, and On the Edge is unlocked.
- **Testing.** Everything in Weekly, plus a **Notes** button on every screen for feedback, the Know-more limits per level in Stook, tuning sliders for On the Edge and tools to clear results.

You can skip the panel by adding `#weekly` or `#testing` to the link, for example:

```
https://YOUR-NAME.github.io/farmers-puzzles/#testing
```

Switch versions any time from the bottom of the home screen.

## How the feedback notes work

Testers tap **Notes**, write a note and tap **Add note**. Each note keeps which game, level and day it's about. When they're done they add their name and work email and tap **Email notes to Dan**, which opens their own mail app with everything filled in. If no mail app opens, **Copy notes** puts the text on the clipboard to paste into an email.

Notes are saved on the tester's own device until they send or clear them. Nothing goes to a server.

To change where the notes go, open `index.html`, search for `FEEDBACK_TO` and change the address.

## Putting it on GitHub Pages (with GitHub Desktop)

1. **Create the repository.** In GitHub Desktop: File → New Repository. Name it `farmers-puzzles`, pick a folder on your Mac (for example `Documents/Hawkstone`), leave everything else as it is and click **Create Repository**.
2. **Add the files.** Open that new folder in Finder (Repository → Show in Finder). Copy in `index.html`, `README.md` and `.nojekyll` from this zip. `.nojekyll` is hidden in Finder; press Cmd+Shift+. to show hidden files.
3. **Commit.** Back in GitHub Desktop, tick all the files in the left list, type a summary such as "First version" in the box at the bottom left, then click **Commit to main**.
4. **Publish.** Click **Publish repository** at the top. Untick "Keep this code private" if you want testers outside your account to open the page (Pages on a free account needs a public repository).
5. **Turn on Pages.** On github.com open the repository → Settings → Pages. Under "Build and deployment" set Source to **Deploy from a branch**, Branch to **main** and folder to **/ (root)**, then Save.
6. **Wait a minute,** refresh the Pages settings and the link appears at the top: `https://YOUR-NAME.github.io/farmers-puzzles/`.

### Updating later

Replace `index.html` in the folder with the new one, then in GitHub Desktop tick it, write a summary, **Commit to main** and **Push origin**. Pages updates within a minute or two. If a phone still shows the old version, close the tab and reopen the link.

## Good to know

- Sound in On the Edge needs the phone's silent switch off on iPhone. It plays on GitHub Pages; it doesn't inside the Claude preview.
- Results, levels, theme and notes live in each person's browser storage. Clearing browser data resets them.
- The standalone On the Edge test repo is separate and still works on its own. This repo carries the same latest version inside the platform.
