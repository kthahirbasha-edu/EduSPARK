EduSPARK Seating Allotment  —  v5 (with Store / Fill Classes / Install)
=======================================================================

WHAT IS IN THIS FOLDER
----------------------
index.html                  -> THE APPLICATION (open this). Everything is
                               inside this single file - the PDF engine is
                               embedded, so it works with or without internet.
EduSPARK_Locked.html        -> Same app, code-protected (obfuscated) build.
manifest.json               -> Makes it installable as an app.
sw.js                       -> Service worker (offline support).
icon-192.png / icon-512.png -> App icons.
eduspark.png / logo.png     -> Original logo.
eduspark-header.png         -> Header logo.
README.md                   -> This file.

NEW IN THIS VERSION
-------------------
1. INSTALL APP button  - Installs EduSPARK on the computer or mobile phone.
   * Android (Chrome): Install app / Add to Home screen
   * iPhone / iPad (Safari): Share -> Add to Home Screen
   * Windows / Mac (Chrome, Edge): install icon in the address bar
   * The button shows step-by-step help if the browser does not offer the
     automatic prompt.

2. STORE button - Saves every class, section, first/last exam number and
   strength, plus your school name, rooms, rows, benches, students per bench,
   centre option, seating mode and room names, into this device's own memory
   (browser localStorage). Nothing is sent anywhere.

3. Permanence - Stored details stay saved after closing the tab/browser,
   after restarting the phone and even offline. They are restored
   automatically the next time the app is opened.

4. DELETE ALL button - Clears everything that was stored on this device.
   It asks for confirmation first. The table on the screen is left as it is.

5. FILL CLASSES button - Brings all stored classes back into the table with
   their exam numbers. Remove any class you do not need, then click
   "Generate High-Low Seating" - the room allotment is made for the remaining
   classes only.

All the earlier features are unchanged: one column = one standard (sections
when a single standard is entered), high-low order, section shuffling,
side / behind rules, sequential & random modes, customizable benches and
students per bench, and the three PDFs (Room Layout, Summary, Exam No -> Room
Map) with the school name in bold at the top centre and the EduSPARK logo.

HOW TO USE
----------
1. Double-click index.html - it opens in your browser and everything works.
2. Enter classes, sections and exam number ranges (First / Last).
3. Click STORE once.  Next time just click FILL CLASSES.
4. Fill school name, date, session, rooms / rows / benches.
5. Click Generate High-Low Seating, then download the PDFs.
6. Use DELETE ALL to wipe the memory when the exam session is over.

HOSTING ON THE WEB (free)
-------------------------
Because everything is in one file, hosting is very easy:
  * Netlify  : go to app.netlify.com/drop and drag this whole folder in.
  * GitHub Pages : upload the folder to a repository, Settings -> Pages ->
                   deploy from branch, then open https://<user>.github.io/<repo>/
  * Vercel / Firebase Hosting / any school web server: upload the folder.
Hosting also enables the automatic install prompt (PWA) and offline mode.
Note: the install prompt needs https:// or localhost - a plain file:// path
still runs the full application, only the automatic install is unavailable.

DATA / PRIVACY
--------------
Stored details never leave the device. They live in the browser's storage for
the folder/website you open the app from. Clearing the browser history /
site data also clears them - use DELETE ALL for a clean reset instead.

support youtube@newEduSPARK
