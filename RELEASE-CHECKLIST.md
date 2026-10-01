# Forge Avatar v0.5.1 — GitHub Release Checklist

The repository files in this starter package are ready to commit.

## 1. Commit the repository files

In GitHub Desktop:

1. Extract this starter ZIP into the root of your local `Stream-Forge-Plugins` repository.
2. GitHub Desktop should show the new files.
3. Commit message suggestion: `Initial Stream Forge plugin catalog`
4. Push / Publish the repository.

## 2. Create the Forge Avatar release

On GitHub.com, open the `Stream-Forge-Plugins` repository and create a new Release.

Use:

- **Tag:** `forge-avatar-v0.5.1`
- **Release title:** `Forge Avatar v0.5.1 — Animation-Only Reliability Cleanup`

Upload these two release assets:

- `Stream-Forge-Forge-Avatar-Plugin-v0.5.1.zip`
- `Stream-Forge-Forge-Avatar-Plugin-v0.5.1.zip.sha256`

Verified package SHA256:

`970703053a04b95a6a5efa873d8cbe4f533304f3d9e9c61ba9dd9cdca0ec929e`

Activation code:

`FAV-7K9M-Q4VX-2RDA`

## 3. Do not commit the plugin ZIP to normal Git history

The root `.gitignore` intentionally ignores `*.zip`.

Use GitHub Releases for packaged plugin downloads. This keeps the repository small while allowing Stream Forge and the website to use one official plugin catalog.

## Future automatic installation

The catalog already contains the release tag, asset names, compatibility list, activation-code SHA256 and package SHA256 needed for the future flow:

`activation code → catalog → GitHub Release → verify → install → unlock`
