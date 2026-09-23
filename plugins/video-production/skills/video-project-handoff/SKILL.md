---
name: video-project-handoff
description: Turn a video project's source footage and client request into an editor-ready handoff with a deliverable count, per-video source assignments, filename map, editing cost, and verified PDF. Use for planning edits from Drive folders or local media, not for rendering finished videos.
argument-hint: "[source folder or Drive URL] [client brief] [editor rate]"
---

# Video Project Handoff

Prepare a practical editing brief from the current project's source media and client instructions. Use **$30 USD per distinct edited video** when the user gives no other rate. Determine the deliverable count for each project; never reuse a prior project's count, filenames, or client details.

## Inventory the source

- Use the supplied folder, client request, and rate. Ask only for information that blocks accurate work.
- Recursively list the source through available filesystem, Drive, MCP, or browser tools. Follow pagination and nested folders before calling the inventory complete.
- Record each media item's current filename, source folder, file type, size, stable source link or path, and file ID when available.
- Separate videos, stills, audio, branding, documents, and system files. Exclude `.DS_Store`, `._*`, thumbnails, proxies, and prior handoff documents from source-media counts unless the user explicitly includes them.
- Do not infer duplicates from filenames alone. Preserve camera sequence numbers and exact extensions.
- Keep original files and folder organization unchanged unless the user asks for file management.

## Review the media honestly

- State the exact review level: metadata only, preview frames, sampled playback, full playback, audio review, or transcript review.
- Preview frames can establish visual content, not dialogue, complete topics, sound quality, sync, full-file usability, or exact timecodes.
- For exact cut points or quotes, review the relevant playback or audio and log filename, source in/out, and exact words. If access prevents this, mark selections provisional instead of inventing them.
- Flag material gaps such as missing logos, inaccessible files, empty camera or audio folders, questionable sound, missing group portraits, or unverified names and titles.

## Define the edits and cost

- Separate the client's explicit request from the recommended scope. Words such as “several” do not establish an exact count.
- Number every distinct creative edit `V01`, `V02`, and so on. Count creative edits separately from raw footage, stills, alternate aspect ratios, captioned or clean variants, and archives.
- Calculate `number of videos x editor rate` and show the unit rate and total. Mark pricing for photos, music, extra versions, project files, and other additions as unspecified unless provided.
- Give every video its own assignment with:
  - title and purpose;
  - target duration and aspect ratio;
  - primary source filenames with verified links or paths;
  - supporting B-roll filenames with verified links or paths;
  - story and editing direction;
  - selection status: verified or provisional.
- Treat shared B-roll as a selection pool. Do not require every listed supporting clip to appear.
- Preserve the meaning and context of speech and reactions.

## Create an editor filename map when useful

- Use a consistent structure such as `PROJECT_YYYYMMDD_SOURCE_OR_CAMERA_ORIGINALNAME.ext`.
- Retain the complete original basename, sequence padding, and extension in the proposed name.
- Check every proposed name for uniqueness, path-length issues, and collisions before any rename.
- Produce a CSV with source folder, current name, proposed editor name, source link or path, stable file ID when available, and rename status.
- If the user authorizes renaming, rename in place and verify each result by readback. Keep an incremental status log so a partial batch can resume safely.
- Never claim a rename succeeded without readback. If the provider denies write access, leave sources unchanged, mark the map `PENDING`, and show both current and proposed names in the handoff.
- Do not duplicate large media files as a workaround for a blocked rename.

## Build the editor handoff

Create a polished PDF using available document or PDF tools. Include:

1. Project identity, client request, recommended deliverable count, rate, total cost, and review limitations.
2. A prominent assignment section for every edit ID with the exact source files to use.
3. Creative direction for hooks, story, captions, branding, sound, music, color, and calls to action.
4. Still-photo selections and raw-footage delivery instructions when requested, kept outside the video count and price.
5. Missing assets, proxy or sync guidance, export settings, and handoff requirements.
6. A source inventory or linked appendix appropriate to the project size.
7. Current and proposed filenames when a rename map exists; label pending names clearly.

Use real source links or paths rather than invented placeholders. Make links clickable when the PDF tool supports them.

## Validate and deliver

- Check the media counts, arithmetic, assignment coverage, filename mapping, source links, and consistency between the summary and detailed assignments.
- Confirm each assigned source exists in the inventory and every mapped filename is unique.
- Render the final PDF to images and inspect every page for clipped text, split rows, overflow pages, unreadable type, and broken links or characters.
- Report the final video count, rate, total, output location, review limitations, unresolved assets, and whether source renames actually succeeded.
- Do not send the handoff to the editor or client unless the user explicitly asks for that communication.

## Example invocation

`/video-production:video-project-handoff Scan this Drive folder, use the attached client request, and create an editor-ready PDF. My editor charges $30 per video. Include the video count, the exact files for each edit, and a filename map.`
