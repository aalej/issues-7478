# Repro for issue 7478

## Versions

node: v22.5.1<br>
firebase-tools: v13.13.3

## Steps to reproduce

1. Set up App Hosting using `firebase apphosting:backends:create --project PROJECT_ID --location us-central1`

```
   i === Import a GitHub repository
   ✔ Connected with GitHub successfully

? Which GitHub repo do you want to deploy? aalej/issues-7478
? Specify your app's root directory relative to your repository /apps/main
? Pick a branch for continuous deployment main
✔ Repo linked successfully!

i === Set up your backend
? Provide a name for your backend [1-30 characters] issues-7478-newer
✔ Name set to issues-7478-newer

⚠ Unable to create a new web app, the project has reached the quota for Firebase apps. Navigate to your Firebase console to manage or delete a Firebase app to continue.
⚠ Firebase web app not set
✔ Successfully created backend!
projects/PROJECT_ID/locations/us-central1/backends/issues-7478-newer

? Do you want to deploy now? Yes
i You may also track this rollout at:
https://console.firebase.google.com/project/PROJECT_ID/apphosting
⠸ Starting a new rollout; this may take a few minutes. It's safe to exit now.
Error: build build-2024-07-23-001 failed to build
```
