# NVIDIA Icon Library for PowerPoint

A PowerPoint add-in that lets you search the NVIDIA marketing icon set and insert icons directly into your slides — no copy/paste, no manual file hunting.

- Search across the full icon library by name, category, or keyword (synonyms supported)
- Insert as **PNG** (200×200 px, ready to drop on any slide), **or**
- Insert as **SVG** (vector — fully resizable and recolorable inside PowerPoint)
- Works in PowerPoint for Windows, Mac, and PowerPoint on the web

---

## Install (for your teammates)

The add-in is delivered as a small XML "manifest" file. Each user installs it once on their machine. After that, **Icon Library** shows up as a button on PowerPoint's Home ribbon.

### Step 1 — Download the manifest

Right-click this link and choose **"Save Link As…"**:

➡ **[manifest.xml](https://raw.githubusercontent.com/talexand88/nvidia-icon-addin/main/manifest.xml)**

Save it somewhere easy to find (your Desktop or Downloads folder is fine).

### Step 2 — Install in PowerPoint

Pick the section that matches your computer.

#### 🪟 Windows (PowerPoint desktop)

1. Open PowerPoint.
2. Go to **Insert** → **Get Add-ins** (also called "My Add-ins" on some versions).
3. Click **Upload My Add-in** (top-right corner of the dialog).
4. Browse to the `manifest.xml` file you saved in Step 1 and choose **Upload**.
5. A new **Icon Library** button appears on the **Home** tab. Click it.

#### 🍎 Mac (PowerPoint desktop)

1. Quit PowerPoint completely (**Cmd + Q**).
2. In Finder, press **Cmd + Shift + G** and paste this path:
   ```
   ~/Library/Containers/com.microsoft.Powerpoint/Data/Documents/wef
   ```
   If the `wef` folder doesn't exist, create it.
3. Drop the `manifest.xml` file into that folder.
4. Reopen PowerPoint. A new **Icon Library** button appears on the **Home** tab.

#### 🌐 PowerPoint on the web

1. Open a presentation at **powerpoint.office.com**.
2. **Insert** → **Add-ins** → **More Add-ins** → **Upload My Add-in**.
3. Choose the `manifest.xml` file from Step 1.

---

## How to use it

1. Click the **Icon Library** button on the **Home** tab — a side panel opens.
2. Type to search (e.g. "ai", "cloud", "robot"), or filter by category.
3. Hover over any icon and choose:
   - **⬇ Insert PNG** — drops a 200×200 px image onto your slide.
   - **↓ Insert SVG** — inserts as a vector you can recolor and resize (or on Mac, downloads the `.svg` file for you to insert via Insert → Pictures → Picture From File).

---

## Updating to a newer version

The add-in pulls its UI from GitHub Pages, so version updates roll out automatically — no re-install needed. If a major manifest change ships, you'll be asked to repeat the install step above.

---

## Troubleshooting

- **"Icon Library" button doesn't appear** → Restart PowerPoint completely (Cmd + Q on Mac, or close all PowerPoint windows on Windows) and reopen.
- **The panel says "Loading icons…" forever** → Check your internet connection — the panel loads icons from `talexand88.github.io`. Hard-refresh by closing and reopening the panel.
- **SVG insert downloads a file instead of inserting it** → That's the expected Mac behavior. Mac PowerPoint doesn't yet support direct SVG injection through add-ins. After the file downloads, use **Insert → Pictures → Picture From File…** and pick the SVG.

---

## Questions / feedback

Reach out to **Tal Alexander** (`taalexander@nvidia.com`).
