# ABC Logistics Inventory Command Center
## Deployment Instructions

---

### Files in This Project

| File | Purpose |
|------|---------|
| `index.html` | Main dashboard – inventory form, table, and chart |
| `about.html` | Developer profile page |
| `DEPLOYMENT.md` | This file |

---

### Option 1 – Netlify Drop (Easiest, ~2 minutes)

1. Go to **[https://app.netlify.com/drop](https://app.netlify.com/drop)** in your browser (no account needed).
2. Make sure all project files are inside a single folder named:
   ```
   ABC_Dashboard_YourName/
   ├── index.html
   └── about.html
   ```
3. Drag the **entire folder** (not individual files) into the Netlify Drop zone.
4. Netlify will instantly give you a public URL like:
   ```
   https://random-name-123.netlify.app
   ```
5. Copy that URL — this is your live website link for the report.

> **Tip:** To get a custom URL, sign up for a free Netlify account and rename the site in *Site Settings → Site details → Change site name*.

---

### Option 2 – GitHub Pages

1. Create a free account at **[https://github.com](https://github.com)**.
2. Click **"+"** → **"New repository"**.
3. Name the repository `ABC_Dashboard_YourName` and set it to **Public**.
4. On your local machine (or using GitHub's web editor), upload both files:
   - `index.html`
   - `about.html`
5. Go to **Settings → Pages**.
6. Under *Source*, select **"Deploy from a branch"** → choose `main` → `/ (root)`.
7. Click **Save**. After ~1 minute, your site will be live at:
   ```
   https://yourusername.github.io/ABC_Dashboard_YourName/
   ```

---

### Testing Locally Before Deployment

**Windows:**
1. Double-click `index.html` to open it in your default browser.
2. Click the "Developer Profile" link to navigate to `about.html`.

**Mac/Linux:**
```bash
cd path/to/ABC_Dashboard_YourName
open index.html        # Mac
xdg-open index.html    # Linux
```

**Using VS Code Live Server (recommended):**
1. Install the "Live Server" extension in VS Code.
2. Right-click `index.html` → **"Open with Live Server"**.

---

### Functional Checklist

Before submitting, verify all features work:

- [ ] Items can be added with Name, Quantity, and Unit Price
- [ ] Pressing **Enter** in any field submits the form
- [ ] Duplicate item names are rejected (case-insensitive)
- [ ] Negative quantities/prices are rejected
- [ ] Non-numeric characters in Qty/Price fields are rejected
- [ ] Total Value (Qty × Price) is displayed correctly
- [ ] Items with Qty < 10 show a red bar and ⚠ Low badge
- [ ] Bar Chart / Pie Chart toggle works
- [ ] **Clear All Items** button deletes all data (with confirmation)
- [ ] Individual items can be removed with the ✕ button
- [ ] Data persists after page refresh (localStorage)
- [ ] Navigation between Dashboard and Developer Profile works on both pages
- [ ] Both pages share the same colour scheme and fonts

---

### Customising the About Page

Open `about.html` and replace the placeholder text with your real details:

| Placeholder | Replace with |
|-------------|-------------|
| `Your Name` | Your full name |
| `BBA – Management Information Systems` | Your actual program |
| `301-XXX-XXX` | Your student number |
| `Spring 2025 – BUS 237` | Current term |
| `Burnaby, BC, Canada` | Your city |
| `yourname@sfu.ca` | Your email |
| `linkedin.com/in/yourprofile` | Your LinkedIn URL |
| `github.com/yourusername` | Your GitHub URL |

---

*BUS 237 – Assignment 2: Vibe Coding*
