# Planner

A calm planner for Android and the PC. It keeps your tasks, calendar, notes, alarms and training in one place, works offline, and stays in sync between your devices through a small server that you own.

> **A personal project, shared as it is.** This page holds the app's installer files, and the phone app checks here for updates. The source code lives in a separate, private repository.

[What it does](#what-it-does) · [Install](#install-on-android) · [Update](#update) · [Getting started](#getting-started) · [Sync and the PC](#sync-and-the-pc-version) · [Privacy](#your-data-and-privacy) · [If something's wrong](#if-somethings-wrong) · [Status](#project-status)

## What it does

| Page | What it's for |
|---|---|
| **Today** | Your day on one screen: routines, tasks, the schedule, and a glance at tomorrow. |
| **Calendar** | Day, 3 days, Week, Month, Year and Agenda views. Drag things to move them. |
| **Tasks** | Tasks with a date, and to-dos without one. |
| **Notes** | Notes, checklists, pictures and videos. A **Links** graph shows how your notes, tasks and events connect. |
| **Training** | A workout plan, a log of each session, and progress charts. It can read your watch's data through Health Connect. |
| **Clocks** (phone) | Alarms, timers, stopwatches and a world clock with the weather. |

Also there:

- **Search** across everything, from the top of every page.
- **Reminders and alarms.** Alarms ring even when the phone is on silent; reminders can keep quiet hours.
- **Home screen widgets**: Today and Upcoming.
- **Categories** with their own colours, **routines** with streaks, and **birthdays**.
- Calendar invites (`.ics` files) open straight in the app.
- Dark and light themes, and a pure black one for OLED screens.

## Install on Android

You need Android 8.0 or newer, and a sync server with its password (see [Sync and the PC version](#sync-and-the-pc-version)).

1. On your phone, open [the latest release](../../releases/latest) and download the `.apk` file.
2. Android asks whether your browser may install apps. Allow it.
3. Open the downloaded file and tap **Install**.
4. Open Planner. Enter your server's address and your sync password, then tap **Connect**.
5. Allow notifications when asked.

For alarms that are never late, open **Settings → Reminders & alarms** and go through its last three rows: **Notification permission**, **Full-screen alarms** and **Battery**.

## Update

When a new version is out, Planner offers it when you open the app. Tap **Update**, then **Install**. Your data stays where it is.

To look for one yourself: **Settings → About → Check for updates**.

## Getting started

- **Add something** with the **+** button. You can type it in plain words, like a title with a day and a time, and Planner fills in the rest.
- **Move around** with the bar at the bottom (on the PC, at the side). Tap the tab you're already on to go back to its start, such as today's date.
- **Hold** an item to see what you can do with it. On the PC, right-click.
- **Deleted something by mistake?** Tap **Undo** right away. After that it waits in **Settings → Data → Trash** for 30 days.
- **Looking for a setting?** Settings has its own search at the top. Type a plain word like *dark*, *backup* or *week*.
- **Make it yours** in **Settings → Appearance**: the theme, the highlight colour, and **Looks to try** for other layouts.
- **On the PC**, the keyboard works too: `Ctrl+F` searches, `N` adds something new, `T` jumps to today.

Settings is in folders: Appearance, Touch and gestures, Calendar & tasks, Notes, Training, Reminders & alarms, Cloud sync, Data and About.

## Sync and the PC version

Every device keeps its own full copy of your data, so Planner works without a connection. When there is one, your devices swap their changes through your sync server, usually within a minute.

- **The server** is a small program that runs on a free Cloudflare account belonging to whoever owns the data. There is no shared Planner service and no sign-up.
- **The PC version** lives on that same server. Open the server's address in Chrome or Edge and enter the sync password. To keep it like a desktop app, use the install button in the address bar.
- **Changing or checking it later:** **Settings → Cloud sync** shows the server, the last sync and how much space is used, with **Sync now** and **Sign out**.

The server's code is part of the private source, so for now Planner can only be used with a server set up by the project's owner.

## Your data and privacy

Your data lives on your devices and on your own server. There is no account, no advertising and no tracking.

**Safety nets**

- The phone saves a full backup every day and keeps the last 14. See **Settings → Data → Back up now** and **Restore from backup**.
- The server keeps one extra copy per day, for 14 days.
- Deleted things stay in the Trash for 30 days. Notes keep their earlier versions for 30 days.
- If the same note was changed on two devices at once, both versions are kept. The second one appears as a "conflicted copy".
- A sync that would delete a large part of your data stops and asks you first.

**What leaves your devices, and when**

| When you… | What is sent | To |
|---|---|---|
| see the weather on an alarm or world clock | the city | Open-Meteo |
| type a place for a task or event | the words typed, and at most your area rounded to about a kilometre | Photon (OpenStreetMap search) |
| hold a web link to see its preview | the link, fetched by your own server | that website |
| paste a Google Maps link as a place | the link, opened by your own server | Google Maps |
| open the app (update check) | only a request for the newest version | GitHub, this page |

Reading your phone's calendars, your contacts' birthdays, Health Connect or screen time is off until you turn it on in Settings, and what it reads is stored like the rest of your data.

## If something's wrong

- **An alarm was late or silent.** Check the three rows at the end of **Settings → Reminders & alarms**. Set the battery row to unrestricted: some phones close apps in the background to save power.
- **The install is blocked.** Android needs your permission for the browser or file app you opened the `.apk` with. It asks once.
- **No update is offered.** **Settings → About → Check for updates**.
- **The phone and the PC show different things.** Open **Settings → Cloud sync** and tap **Sync now**. If it says deletions are waiting, choose **Delete them** or **Restore them**.
- **Something is gone.** Look in **Settings → Data → Trash**, then **Restore from backup**.
- **The app misbehaved.** **Settings → Data → Problem log** keeps a short list of what went wrong on that device, which you can copy.

## Project status

Planner is in daily use and changes often, sometimes several times a week. Each release on this page has a few lines on what changed.

It is built around one person's needs. Two parts, the Training plan and the Reading folder in Notes, are filled from the PC with small tools from the private source, and stay empty without them. There is no Play Store or iPhone version, and no support is promised.
