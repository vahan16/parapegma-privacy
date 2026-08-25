# Parapegma — privacy policy and support

The two published pages for **Parapegma**, a trip planner that costs out the
moving.

| page | url | in the listing as |
| ---- | --- | ----------------- |
| privacy policy | **https://vahan16.github.io/parapegma-privacy/** | Privacy Policy URL |
| support | **https://vahan16.github.io/parapegma-privacy/support.html** | Support URL |

Apple requires both, and rejects a Support URL that turns out to be a privacy
policy under another label. `vahan16/plumula-privacy` holds the same pair.

## Do not edit `index.html` or `support.html`

They are generated. Both are authored in the app's own repository — the policy
at `worker/privacy.ts`, the support page at `worker/support.ts` — and written
here by:

```bash
node scripts/build-privacy.mjs ../parapegma-privacy
node scripts/build-support.mjs ../parapegma-privacy
```

Run whichever you changed. Editing these copies means the app's repository and
the published pages disagree about what the app does, which is the one failure
a privacy policy cannot have — and a support page that names a button the app
does not have is not much better. Change it there, regenerate, commit here.

Pushing to `main` deploys it — see `.github/workflows/pages.yml`.
