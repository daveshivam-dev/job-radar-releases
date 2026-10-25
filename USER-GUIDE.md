# Job Radar user guide

Job Radar collects new job openings from company career sites and job boards into one list on your computer.
This guide takes about 5 minutes to read.

- [1. Install](#1-install)
- [2. First start](#2-first-start)
- [3. Your job list](#3-your-job-list)
- [4. Companies](#4-companies)
- [5. Job boards](#5-job-boards)
- [6. Fix issues](#6-fix-issues)
- [7. Settings](#7-settings)
- [8. Updates](#8-updates)
- [9. Feedback and privacy](#9-feedback-and-privacy)
- [10. Uninstall](#10-uninstall)
- [11. If something goes wrong](#11-if-something-goes-wrong)

## 1. Install

You need a Mac (Apple silicon or Intel, macOS 11 or newer) or a Windows 10 or 11 computer, and an internet
connection. Nothing else: Job Radar brings its own copy of Python and downloads it once while installing.

1. Open the **[latest release](../../releases/latest)** and download **`Job-Radar-<version>-setup.zip`**.
   That is the only file you need. The other files are used by automatic updates, and "Source code" holds only
   the text of the download page.
2. Unzip it. You get a folder called `job-radar`.

**Mac**

1. Open **Terminal**: press Cmd + Space, type `Terminal`, press Enter.
2. Type `bash ` (with a space after it), drag the file `install_mac.sh` from the `job-radar` folder into the
   Terminal window, and press Enter.
3. Wait about 2 minutes. When asked about a daily check, press **Y** to look for new jobs every morning at 8:45,
   even when the app is closed.

Job Radar opens and is now in your **Applications** folder. Drag it to the Dock to keep it there.

**Windows**

1. Double-click **`install_windows.bat`** in the `job-radar` folder.
2. If Windows shows "Windows protected your PC", click **More info**, then **Run anyway**. The installer is not
   signed yet; this is expected.
3. Wait about 2 minutes, then answer the daily check question with **Y** or **N**.

Job Radar is now on your Desktop and in the Start menu.

You can delete the downloaded zip and the `job-radar` folder afterwards.

## 2. First start

1. The **Welcome** window asks whether you want to share anonymous usage data. Either answer is fine; see
   [Feedback and privacy](#9-feedback-and-privacy).
2. Open **Settings** and choose:
   - **Countries to search**, and whether you want **Remote jobs** too
   - **Languages you can work in** (this drives the "English is enough" filter)
   - **Role types to look for**, for example Software, Data or Finance
3. Click **Refresh** at the top. The first refresh reads every company and board and takes a few minutes.
   After that, Job Radar refreshes by itself every 6 hours while it is open.

## 3. Your job list

The **Jobs** tab shows every opening that matches your settings, newest first.

- **Search** title, company or city in the box at the top (shortcut: press `/`).
- **Filters** on the left:
  - **Posted**: Today, 3, 7, 14 or 30 days, or All
  - **Work type**: Remote, Hybrid or On-site, with office days when the ad says
  - **Country**, **City**, **Seniority**, **Role**
  - **Language**: "English is enough", "Local language needed" or "Not clear"
  - **Found on**: a company's own site or a job board
  - **Salary**: from the ad, or a market estimate (marked with ≈)
  - **Show only**: Focus roles, jobs in your languages, new since last refresh, saved, applied
  - **Reset filters** clears them all
- **Sort**: newest first, highest salary, or company A to Z.
- Click a job to see its details: work type, office days, salary, languages and seniority, each with the
  sentence from the ad it came from, and **View source** to open the original ad.
- On each job:
  - **Star**: save it for later
  - **Tick**: mark it as applied
  - **Hide**: not interested (bring hidden jobs back with "Include hidden jobs" under Show only)
- **Export list** saves the jobs you see as a spreadsheet file (CSV) you can open in Excel or Numbers.

## 4. Companies

The **Companies** tab lists every company Job Radar reads, with its hiring system, status and number of jobs in
your countries. It starts with 140+ companies.

To add one, click **Add company** and paste its careers page or any of its job ads. Job Radar works out the rest,
including small local companies with only their own website. Search the list with **Search companies**.

## 5. Job boards

The **Job boards** tab shows popular boards for the countries you search.

- Boards marked **Reads automatically** add their jobs to your list on every refresh. Tick the ones you want.
- Some need your own free key: click **Get a free key**, then paste it and click **Save key**.
- The other boards don't allow automated reading. For those, Job Radar opens a ready-made search in your browser
  with your search words, city and dates filled in. **Open all** opens every ticked board at once.

## 6. Fix issues

Company career sites change. When a company's feed stops working, Job Radar first tries to repair it by itself.
What it can't fix appears in **Fix issues** with clear steps, for example **Find careers page** to paste the new
address, or **Pause company** to stop reading it. **Check problem companies again** retries them all.

## 7. Settings

Changes are saved as you make them.

- **Countries to search**, **Remote jobs**, **Languages you can work in**, **Role types to look for**
- **Focus roles**: words that matter most to you; matching jobs get a Focus tag and their own filter
- **Automatic refresh**: refresh when the app opens, how often while it is open, notifications for new jobs
  (Mac), and how many days of jobs to show by default
- **How salaries are shown**: "In the ad" means the company published it; "Market estimate" (marked with ≈)
  comes from public salary data for the role, level and city
- **Your data**: **Open data folder** shows where your jobs and settings are stored
- **Help improve Job Radar**: switch anonymous usage data on or off
- **Updates**: check for updates and see what's new
- **Privacy note** and **Licence**

## 8. Updates

Job Radar checks for new versions once a day. When one is out, an **Update** button appears at the top: one
click, about a minute, then **Restart now**. Your jobs, marks and settings stay. If a new version ever fails to
start, Job Radar goes back to the previous one by itself.

## 9. Feedback and privacy

- Click **Feedback** at the top to send an idea or a problem. Every message is read. Leave your email only if you
  want an answer.
- After 2 and 4 weeks, Job Radar asks 3 short questions. Your answers decide what gets built next.
- Your jobs, searches and settings stay on your computer. Anonymous usage data is shared only if you said yes, and
  never includes your name, CV, searches or the jobs you look at. Details: [PRIVACY.md](PRIVACY.md).

## 10. Uninstall

**Mac:** in Terminal, type `bash `, drag `uninstall_mac.sh` from the `job-radar` folder into the window and press
Enter. Your jobs and settings are kept; add ` --all` before pressing Enter to delete them too.

**Windows:** delete the Job Radar shortcuts from the Desktop and Start menu, delete the folder
`%LOCALAPPDATA%\Job Radar`, and in **Task Scheduler** delete "Job Radar daily check" if you turned it on.

## 11. If something goes wrong

| What you see | What to do |
|---|---|
| "Windows protected your PC" | Click **More info**, then **Run anyway** |
| The installer stops at "Downloading the Python..." | Check your internet connection and run the installer again |
| "The window library did not install" | Job Radar still works and opens in your web browser instead |
| An update shows an error in Settings > Updates | Download the latest setup zip and install again; your jobs and settings stay |
| A company shows no jobs | Open **Fix issues** and follow the steps there |
| Anything else | Click **Feedback** and describe what happened |
