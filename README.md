# Birthday website - Vercel (static, single file)

index.html must sit at the TOP LEVEL of the folder you deploy (not inside another folder).
Everything (design, 5 photos, background song) is inside index.html. No build step.

## Deploy with the CLI
    cd <this folder>          # the folder that directly contains index.html
    npm install -g vercel
    vercel --prod             # press Enter on every question (code directory = ./)

## Deploy by drag and drop
Unzip first. Drag the unzipped folder (the one that directly contains index.html) onto vercel.com/new.
Do NOT upload the .zip file itself.

## If you ever see "404 NOT_FOUND"
- index.html is inside a sub-folder, or you uploaded the .zip itself.
- In Vercel: Project -> Settings -> General -> Root Directory must be the folder that contains index.html.
- Settings -> Build & Development: Output Directory empty (or "."), Framework Preset "Other".
