# Your Vinaya Notes Module

**Fork this reprository to create your own Vinaya Notes Module!**

## Steps

1. Fork this repo
2. Fill in the `metadata.yaml` file with your folder's information
3. Update this `README.md` with your own introduction to your module. Be sure to include any relevant copyright information!
4. Copy your notes over to this repo (treat the repo root directory as your module's root directory, i.e. this repo could live inside a vault)
5. When you're ready, set the "if" in `.github/workflows/release.yaml` to "true"
6. Commit and push your changes to GitHub
7. You'll see a new release created with your notes in a `.zip` file alongside a `.vnm` module file

## How it works

This repo comes with a GitHub Actions script (at .github/workflows/release.yaml)
which will automatically create a new GitHub Release with your Module every time
you push an update to the `main` branch.

Your latest .vnm file will always live at `https://github.com/your-name/your-repo-name/releases/latest/download/manifest.vnm`

## Customization

If you'd like to add a custom build step, just modify the `release.yaml` file to add whatever build steps you need.
The `Canon (Pali)` folder, for example, uses a custom `generate.py` python script to build its folder.
You can see its build script [here](https://github.com/obu-labs/pali-vinaya-notes/blob/main/.github/workflows/build.yaml).

