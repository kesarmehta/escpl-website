ESCPL WEBSITE — DEPLOY TO GODADDY
=================================

WHAT'S IN THIS FOLDER
  index.html      the website (this is your home page)
  support.js      required runtime file — must sit next to index.html
  img/            all 72 photographs and brand logos, compressed for web

Keep the structure exactly as it is. index.html and support.js at the top
level, images inside img/. Do not rename anything.


BEFORE YOU START — CHECK YOU HAVE HOSTING
  A domain on its own has nowhere to upload files to. In GoDaddy, open
  "My Products". You need a Web Hosting (cPanel / Linux) plan listed there,
  not only the domain. If you only see the domain, buy the cheapest cPanel
  hosting plan first.


STEP 1 — OPEN THE FILE MANAGER
  GoDaddy -> My Products -> Web Hosting -> Manage -> cPanel Admin
  In cPanel, open "File Manager", then open the folder: public_html


STEP 2 — CLEAR THE PLACEHOLDER
  public_html usually contains a GoDaddy "coming soon" or default
  index.html. Delete that file (or rename it to old-index.html).


STEP 3 — UPLOAD
  Easiest: zip this whole folder on your computer, then in File Manager
  click Upload and send the .zip into public_html. Right-click the
  uploaded .zip -> Extract. Then delete the .zip.

  Important: after extracting, index.html, support.js and img/ must be
  directly inside public_html — NOT inside public_html/deploy/. If they
  landed in a sub-folder, open it, select all three, and use Move to
  shift them up into public_html.


STEP 4 — POINT THE DOMAIN
  If the hosting plan is already tied to electricalswitchgears.in, you're
  done — visit the domain. If not: cPanel -> Domains -> set
  electricalswitchgears.in as the primary domain pointing at public_html.
  DNS changes can take up to a few hours to appear worldwide.


STEP 5 — CHECK
  Visit https://electricalswitchgears.in and confirm:
    - the hero carousel slides
    - the 24 brand cards open when clicked
    - the six "on the rack" carousels rotate
    - the awards, certificates and client collages all load


ADD HTTPS (FREE)
  cPanel -> Security -> SSL/TLS Status -> Run AutoSSL. Then in
  "Force HTTPS Redirect" turn it on so visitors always get the secure site.


NOTE ON YOUR TWO DOMAIN NAMES
  You own electricalswitchgears.in (plural). Your old site runs on
  electricalswitchgear.in (singular). If you own both, point the old one
  at the new one so nobody lands on the outdated site.


UPDATING THE SITE LATER
  Ask me for a fresh deploy folder whenever the design changes, then
  re-upload — replacing index.html alone is enough unless images changed.


WHAT STILL NEEDS YOUR ATTENTION
  - All brochure and catalogue buttons open Google Drive links. Anyone
    visiting must be able to view those files, so in Drive set each one to
    "Anyone with the link - Viewer". Otherwise visitors see a
    permission-request screen.
  - A few brands (ESC Plast, Bajaj) still open an email instead of a PDF.
  - The rack carousels have placeholder frames in slides 2 to 5 for some
    categories. Send photographs and I'll fill them in.
