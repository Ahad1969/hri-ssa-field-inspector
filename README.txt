HRI SSA FIELD INSPECTOR — VERSION 1.3 PILOT
===========================================
16 sites: 14 HRI plus IP 183 and IP 184. Android-ready progressive web app.

UPGRADE FROM VERSION 1.2
1. Export a FULL JSON BACKUP from your current app and store it safely outside the app folder.
2. Extract all Version 1.3 files into your existing app folder, replacing the program files.
3. Open index.html from the SAME folder/path in Chrome. Existing desktop IndexedDB records should remain available.
4. Check HRI-N26's test issue and photo; verify photo dropdown now shows issue CODE + TITLE.
5. Check Voice tab and full backup. If existing data does not appear, STOP: do not restore until we check the browser origin/path and backing up the old data.

NEW IN V1.3
- Per-site Voice tab: Record (max 2 minutes / 8 MB), stop, replay and delete.
- Title, optional link to a safety issue and editable transcript for each voice note.
- Optional browser speech recognition; may require internet and may send audio to the speech provider.
- Existing Android keyboard dictation may enter text in the transcript field.
- Full JSON backup includes embedded voice audio and transcripts; old v1 backup data is supported.
- Photo issue dropdown shows readable issue code and title instead of UUID; full photo preview.
- No external survey-data server or sync is used.

IMPORTANT LIMITATIONS
Opening index.html with file:// is only a preview. Microphone permissions may be blocked.
For reliable recording, install/serve the PWA on HTTPS (or use localhost in a desktop test).
Speech-to-text does NOT automatically transcribe saved audio. Click optional speech-to-text to
capture new microphone dictation, or use Android keyboard microphone in the transcript field.
Speech recognition can involve internet or vendor cloud processing. Avoid confidential speech
unless authorised. Notes and photos stay in local application storage unless manually exported.
Audio can grow JSON backups; make backups after each visit. Chrome/browser clearing may erase data.
The browser environment has not yet been field-tested for recording or offline mode.

PROPOSED ANDROID DEPLOYMENT
Upload only static PROGRAM files to HTTPS hosting, never personal backups, recorded audio or
site records. Open site on Android Chrome, add/install to Home Screen, grant microphone permission,
and verify offline app loading and backup/restore before relying on it.

TEST
- Open HRI-N26, confirm old issue and photo.
- Confirm photograph link shows HRI-N26-ISS-001 and title.
- Voice: create 5-second recording, stop, play it, write transcript, link to test issue.
- Close/reopen, confirm recording + transcript remain.
- Export JSON backup and verify it can be restored to a SEPARATE test installation.

Version 1.3 pilot. No guarantee of automatic offline transcription or original audio export.
