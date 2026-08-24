# Parapegma — privacy policy

The published privacy policy for **Parapegma**, a trip planner that costs out the
moving.

**https://vahan16.github.io/parapegma-privacy/**

That URL is what the App Store and Google Play listings point at.

## Do not edit `index.html`

It is generated. The policy is authored in the app's own repository, at
`worker/privacy.ts`, and written here by:

```bash
node scripts/build-privacy.mjs ../parapegma-privacy
```

Editing this copy means the app's repository and the published page disagree
about what the app does, which is the one failure a privacy policy cannot
have. Change it there, regenerate, commit here.

Pushing to `main` deploys it — see `.github/workflows/pages.yml`.
