# wilyhq/scoop-bucket

Scoop bucket for [wily](https://wily.bot).

```powershell
scoop bucket add wilyhq https://github.com/wilyhq/scoop-bucket
scoop install wilyhq/wily        # desktop app + CLI (Start menu shortcut, `wily` on PATH)
scoop install wilyhq/wily-cli    # only the CLI, for a machine without the app
```

Install one of the two: both put `wily` on `PATH`. `scoop bucket add` needs git (`scoop install git`).

Both update themselves from `updates.wily.bot` (`wily self-update`, or Settings → Updates in the app);
`scoop update wily` works too. Binaries are downloaded from `dl.wily.bot`; this repository holds only
the manifests. Windows x64 only for now; builds are not code-signed yet.
