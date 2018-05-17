# README

Test the file watcher by changing the `README.md` on `feature` branch, then
executing the `repro` script.

NOTE: the `repro` script is intentionally kept very simple and will break on
merge conflicts. The simplest way to avoid merge conflicts is to add new text
to the README as new text lines.

1. checkout `feature`
2. open this readme in atom
3. edit and commit to `feature`
4. run `repro`
5. the readme in atom will be reloaded to the last version from `deploy` branch
6. the readme on disk will be the latest version from `feature` branch

--- insert here ---

more text
and more
--- until here ----
