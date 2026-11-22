# wilyhq/scoop-bucket

Scoop bucket for [wily](https://wily.bot).

Without git (no bucket, no 7-Zip needed):

```powershell
scoop install https://raw.githubusercontent.com/wilyhq/scoop-bucket/main/bucket/wily.json      # app + CLI
scoop install https://raw.githubusercontent.com/wilyhq/scoop-bucket/main/bucket/wily-cli.json  # only the CLI
```

With git:

```powershell
scoop bucket add wilyhq https://github.com/wilyhq/scoop-bucket
scoop install wilyhq/wily        # desktop app + CLI (Start menu shortcut, `wily` on PATH)
scoop install wilyhq/wily-cli    # only the CLI, for a machine without the app
```

Install one of the two: both put `wily` on `PATH`. `scoop bucket add` needs git (`scoop install git`).

Both update themselves from `updates.wily.bot` (`wily self-update`, or Settings → Updates in the app);
`scoop update wily` works too. Binaries are downloaded from GitHub Releases of [wilyhq/wily](https://github.com/wilyhq/wily/releases); this repository holds only
the manifests. Windows x64 only for now; builds are not code-signed yet.
