# Git Changes & Deployment Guide

This note is the handoff sheet for the GitHub Pages profile package. It keeps the workflow simple: edit only the GitHub Pages copy, keep Netlify untouched, and push only the files that belong in the published profile.

---

## Repository
- **GitHub repo:** [SaqCompanyProfile](https://github.com/mujtaba9598-hasan/SaqCompanyProfile)
- **Primary branch:** `main`
- **GitHub Pages target:** the repository root on `main`
- **Live pages:**
  - [Corporate Profile](https://mujtaba9598-hasan.github.io/SaqCompanyProfile/SAFA_AL_QUDRA_Corporate_Profile.html)
  - [Signature Edition](https://mujtaba9598-hasan.github.io/SaqCompanyProfile/SAFA_AL_QUDRA_Signature_Edition.html)

---

## Local Packages

### GitHub Pages Package
- **Folder:** [SaqCompanyProfile_temp](file:///c:/Users/Mujtaba%20Hasan/Downloads/Saqtech/SaqCompanyProfile_temp)
- **Editable files:**
  - [SAFA_AL_QUDRA_Corporate_Profile.html](file:///c:/Users/Mujtaba%20Hasan/Downloads/Saqtech/SaqCompanyProfile_temp/SAFA_AL_QUDRA_Corporate_Profile.html)
  - [SAFA_AL_QUDRA_Signature_Edition.html](file:///c:/Users/Mujtaba%20Hasan/Downloads/Saqtech/SaqCompanyProfile_temp/SAFA_AL_QUDRA_Signature_Edition.html)
- **Assets folder:** [images/](file:///c:/Users/Mujtaba%20Hasan/Downloads/Saqtech/SaqCompanyProfile_temp/images/)

### Netlify Package
- **Folder:** [SaqCompanyProfile_Netlify](file:///c:/Users/Mujtaba%20Hasan/Downloads/Saqtech/SaqCompanyProfile_Netlify)
- **Rule:** do not edit this package unless the user explicitly says so
- **Contents:** landing page, profile HTML files, and optimized image assets

---

## Current Profile Layout
- Two long-form company profiles, each laid out as an A4 page sequence.
- The Corporate and Signature editions share the same content structure.
- Images are embedded as file references, not as inline base64.
- The page sequence includes cover, CEO message, contents, company overview, services, partners, project pages, factory, HSE, and contact pages.

---

## Recent Git History
- The remote history includes the cleanup commit that removed the lock screen, stripped copy/print protection, and moved the embedded images into files.
- The GitHub Pages package now uses original PNG/JPEG assets in `images/`.
- Netlify keeps its separate optimized version and should be left alone unless the user requests changes there.

---

## Latest Removals
These are the most recent page-level edits already made in the GitHub Pages package:

- Removed the `Water Feature` and `Decorative CNC Perforated Sheet` project page.
- Removed `Extended Skylight`.
- Removed `Extended Skylight with Glass Top and Front`.
- Removed `Wall Mirrors`.
- Removed `Ceiling Mirrors`.
- Removed the two `Stainless Steel Decorative Works` cards on the later project spread.
- The remaining project pages and margins were kept intact.

Current profile count after these removals and the June project insert: `25` pages in each edition.

---

## GitHub Pages Change Rules
1. Edit only `SaqCompanyProfile_temp`.
2. Keep the Netlify folder unchanged.
3. Preserve original PNG/JPEG formats unless the user asks for a different format.
4. Remove or add only the exact cards, logos, or pages the user names.
5. Do not shift margins, page order, or surrounding layout unless a change requires it.
6. Stage only the files that belong to the GitHub Pages update.
7. Commit with a short, descriptive message.
8. Push to `origin/main`.
9. Confirm the remote head matches the new commit.

---

## Push Checklist
Use this when another agent is ready to publish the GitHub Pages update.

1. Check `git status` inside `SaqCompanyProfile_temp`.
2. Review the diff and stage only the intended files.
3. Commit the update with a concise message.
4. Push the commit to `origin/main`.
5. Verify the new commit is the branch head.
6. Leave `SaqCompanyProfile_Netlify` unchanged.
7. If more removals are requested, repeat the same edit-and-push flow only in `SaqCompanyProfile_temp`.

---

## June 2026 Insert
- Source folder: `SaqCompanyProfile_temp/13 June 2026`
- Project order: `Project G02 Palm jumeirah`, `Saadiyat Island Abu Dhabi`, `The field Dubai`, `The lakes Dema 3`
- Add the pages in that order before the factory/HSE section.
- Keep the page design unchanged: same margins, same page size, same footer style, same page numbering.
- Use the original `JPEG` images copied into `SaqCompanyProfile_temp/images`.
- Use the text from each folder’s `BBQ.txt` as the card data for location and item titles.
- When ready to push, stage only the GitHub Pages files in `SaqCompanyProfile_temp` plus this deployment note if it changed.
- Commit, push to `origin/main`, and verify the remote head after push.

## Agent Handoff
If you are another agent reading this file, follow these rules exactly:
- Read this document first before making any changes.
- Edit only the GitHub Pages package in `SaqCompanyProfile_temp`.
- Do not touch `SaqCompanyProfile_Netlify`.
- Keep all images in their original `PNG` / `JPEG` form.
- Apply only the exact add/remove requests already listed by the user.
- Preserve layout, page order, margins, and spacing unless the user says otherwise.
- After the local edits are ready, stage, commit, and push only the GitHub Pages files.
- Do not invent new changes, cleanup, or redesign work on your own.

---

## Git Commit Instructions
Use these exact steps when the local changes are ready to publish:
1. Review `git status` and confirm only `SaqCompanyProfile_temp` and this note are changed.
2. Stage only the intended GitHub Pages files.
3. Commit with a short message that matches the change.
4. Push to `origin/main`.
5. Confirm the remote branch head matches the new commit.
