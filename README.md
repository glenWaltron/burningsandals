# DJ Burning Sandals website

A single page site hosted free on GitHub Pages at burningsandals.com.

## What's in this folder

| File | What it does |
|---|---|
| index.html | The whole website |
| images/ | Promo photo and the three GIFs (you add these, see step 1) |
| CNAME | Tells GitHub to serve the site at burningsandals.com |
| .nojekyll | Tells GitHub to serve the files as they are |

## Step 1. Save your images from Squarespace

Do this before cancelling anything, because these links stop working once the Squarespace site is gone. Open each link, right click, save, and rename exactly as shown into the images folder.

| Save as | Link |
|---|---|
| images/promo.jpg | https://images.squarespace-cdn.com/content/v1/5e4cb3a3227ba62de80be83e/990b5217-7852-4811-8869-9a2a595a644e/for-web-BURNING-SANDALS-PROMO-IMAGE.jpg |
| images/sandals-1.gif | https://images.squarespace-cdn.com/content/v1/5e4cb3a3227ba62de80be83e/1616037633234-QLSFCHDAU9RSPMWKYL6E/burning+sandals+1s.gif |
| images/sandals-2.gif | https://images.squarespace-cdn.com/content/v1/5e4cb3a3227ba62de80be83e/1616037522979-BYR1S3JPS94IFJHMR18U/burning+sandals+2s.gif |
| images/sandals-3.gif | https://images.squarespace-cdn.com/content/v1/5e4cb3a3227ba62de80be83e/1616037895096-KO9W6QD4XI0G2DPG8JA9/burning+sandals+3s.gif |

## Step 2. Add your mix links

Open index.html in any text editor, search for MIXES, and paste each mix's Mixcloud or SoundCloud page link between the quote marks after url. Mixcloud and SoundCloud links play right on the page. A mix with no link still shows, just without a play button.

## Step 3. Put it on GitHub

1. Sign in at github.com (or make a free account).
2. Click New repository. Name it burningsandals, set it to Public, click Create.
3. Click "uploading an existing file", drag in everything from this folder (including the images folder), click Commit changes.
4. Go to Settings, then Pages. Under Source pick "Deploy from a branch", choose main and / (root), click Save.
5. A minute later the site is live at yourusername.github.io/burningsandals. Check it there first.

Note: .nojekyll starts with a dot so your computer may hide it. The site works fine without it if it gets left behind.

## Step 4. Point burningsandals.com at GitHub

Find where the domain is registered (most likely Squarespace Domains). In its DNS settings:

1. Delete the existing Squarespace A records and the www CNAME record.
2. Add four A records with host @ pointing to:
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
3. Add one CNAME record with host www pointing to yourusername.github.io
4. Leave any MX records alone (none needed for a Gmail address anyway).

Back on GitHub in Settings, Pages, type burningsandals.com in Custom domain and save. Once the check goes green (anything from ten minutes to a day), tick Enforce HTTPS.

## Step 5. Cancel the Squarespace site plan

Only once the new site loads at burningsandals.com with the padlock showing. Cancel the website subscription, keep the domain. The domain renewal is a small separate yearly fee. If you want to cut that too, you can transfer the domain to a cheaper registrar such as Cloudflare or Porkbun later.

## Making changes later

On GitHub, open index.html, click the pencil icon, edit, Commit changes. The live site updates within a minute or two.
