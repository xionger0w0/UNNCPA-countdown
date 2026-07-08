# UNNCPA Online Recruitment Countdown

This countdown page was created with the assistance of AI, based on my own requirements, design decisions, testing, and final selection. I used AI as a practical development tool to help turn the idea into a working webpage, while I defined the purpose, reviewed different versions, tested the page on desktop and mobile, and decided how it should be used in Feishu.

The page was made for UNNCPA Autumn Recruitment 2026. Its main purpose is to provide a clear and real-time reminder of the online application deadline inside our Feishu knowledge base.

## Purpose

Instead of only writing the deadline in text, I wanted the recruitment page to include something more direct and visible.

The application deadline is:

September 23, 2026, 12:00 PM

The page shows a live countdown in days, hours, minutes, and seconds. This makes the deadline easier to notice, especially for students who are browsing the recruitment information on their phones.

## Why v2 Was Chosen

The first version had a more complete desktop layout, but it was not ideal when embedded into Feishu, especially on mobile. It required more vertical scrolling, which made the countdown less immediate.

For this reason, I chose v2 as the main version. It keeps the essential information while making the layout more compact:

- UNNCPA Autumn Recruitment
- Online recruitment countdown
- Application deadline
- Days, hours, minutes, and seconds
- A short reminder message

Compared with the first version, v2 is cleaner, lighter, and more suitable for Feishu embedding and mobile viewing.

## File Notes

The local folder contains several versions:

- `v0.1.html`: the first version, better suited for desktop viewing.
- `v0.2.html`: the second version, which is the version I chose for Feishu.

When developing locally, the second version was originally named `compact.html`. After uploading it to GitHub, I renamed it to `v0.2.html`.

## Feishu Link

The GitHub Pages link for the selected version is:

https://xionger0w0.github.io/UNNCPA-countdown/v0.2.html

This link can be inserted into Feishu as a webpage embed, link preview, or web card. For the recruitment knowledge base, v2 is the preferred version because it is easier to view on mobile.

## How to Update the Deadline

If the recruitment deadline changes in the future, update this line in the HTML file:

```js
const deadline = new Date("2026-09-23T12:00:00+08:00").getTime();
```

For example, if the deadline becomes September 25, 2026 at 8:00 PM, change it to:

```js
const deadline = new Date("2026-09-25T20:00:00+08:00").getTime();
```

After editing the file, upload the updated version to GitHub again so that GitHub Pages can publish the change.

## What Happens After the Deadline

The countdown will not show negative numbers. Once the deadline has passed, the timer stops at zero and the message changes to:

Online recruitment has closed. Thank you for taking the time to learn about UNNCPA. We hope to see you again in future activities.

This keeps the page clear and presentable even if someone opens the link after the deadline.

## Why This README Exists

This is a small webpage, but it is a useful part of the recruitment workflow. I kept this README so that I, or future UNNCPA members, can quickly understand what each file is for and how to update the page when needed.

If a similar countdown page is needed in the future, v2 can be reused by updating the deadline, title, and reminder message.

