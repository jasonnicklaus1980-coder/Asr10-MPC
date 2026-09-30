# Building the MPC plugins on GitHub (no tools to install)

1. Sign in at github.com, click **+ > New repository**, name it (private is fine), **Create repository**.
2. On the empty repo page click **uploading an existing file**. Drag the *contents* of this unzipped folder into the
   page (all folders at once: .github, src, mpc, scripts, ...). Wait for the list to finish, then **Commit changes**.
3. Check that the repo shows a `.github/workflows/arm.yml` file. If the `.github` folder is missing (some systems
   hide it from drag and drop): **Add file > Create new file**, type `.github/workflows/arm.yml` as the name, paste
   the contents of the arm.yml you were given, and commit.
4. Open the **Actions** tab. The *ARM build* run starts by itself (or pick it and press **Run workflow**).
   It takes roughly 5-15 minutes.
5. When it is green, open the run and download **mpc-armv7-packages** at the bottom: it holds
   `ASR10-1.2.0-mpc-armv7.zip` (the effect) and `ASR10-Instrument-0.1.0-mpc-armv7.zip` (the instrument).
6. If a step is red, click it, copy the log text, and send it to me.
