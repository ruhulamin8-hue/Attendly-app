# Attendly

A simple attendance app with four windows:

1. **Attendance**: pick a date and subject, then mark each student present or absent.
2. **Import**: import students from an Excel or CSV file, add subjects, and choose the semester.
3. **Dashboard**: attendance percentage overall, by subject and by student.
4. **Developer**: details about you and the app.

Data is stored on the device (localStorage inside the app).

## Before you build

Open `www/index.html` and edit the `DEV` block near the top of the script with your name, role, college, email and GitHub username.

## Get the APK from GitHub

1. Create a new GitHub repository and push this folder to the `main` branch.
2. Open the **Actions** tab. The **Build APK** workflow runs on every push. You can also run it with **Run workflow**.
3. When it finishes, open the run and download **attendly-debug-apk** under Artifacts.
4. Unzip it and install `app-debug.apk` on your phone (allow installs from unknown sources).

## Excel format

| Roll No | Name |
|---------|------|
| CS301   | Aarav Sharma |
| CS302   | Diya Patel |

Choose the semester on the Import screen before selecting the file. Importing again with the same roll number updates the name.

## Change the app name or id

Edit `capacitor.config.json` (`appId`, `appName`) before the first build.
