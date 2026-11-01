PLANNER APP - GitHub setup

A) Put the app online (GitHub Pages)
1. Create a free GitHub account, then create a NEW PUBLIC repository named "planner".
2. In the repository: Add file > Upload files. Unzip planner-app.zip first and upload the files INSIDE the folder
   (index.html, sw.js, manifest.webmanifest and the 4 icon .png files), not the folder itself. Commit.
3. Settings > Pages > Build and deployment: Source = "Deploy from a branch", Branch = main, folder = / (root). Save.
4. After a minute your app is at https://YOURNAME.github.io/planner/
5. Open it on phone and laptop and install it (iPhone: Share > Add to Home Screen; Android/Chrome: Install app).

B) Sync between devices (a second, PRIVATE repository holds your data)
1. Create another repository named "planner-data", set to PRIVATE, and tick "Add a README file".
2. GitHub > your profile picture > Settings > Developer settings > Personal access tokens > Fine-grained tokens > Generate new token.
   - Repository access: Only select repositories > planner-data
   - Permissions > Repository permissions > Contents: Read and write
   - Choose an expiry date, generate, and copy the token (starts with github_pat_).
3. In the app: Settings > Sync between devices. Enter yourname/planner-data and paste the token. Save and sync.
4. Repeat step 3 on your other device with the same repository and token.

Updating the app later: upload the new files to the "planner" repository (Add file > Upload files, replace the old ones).
