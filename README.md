# README

Test the file watcher by changing the `README.md` on `feature` branch, then
executing the `repro` script.

NOTE: the `repro` script is intentionally kept very simple and will break on
merge conflicts. The simplest way to avoid merge conflicts is to add new text
to the README as new text lines.

1. git checkout `feature`
2. open this README in atom
3. add some text at the end
4. commit new version of README to `feature` branch
5. run `repro`, which will
    1. switch to `deploy` branch
    2. previous version of the README will be loaded in atom
    3. merge `feature` into `deploy`
    4. the new version of the README **won't be loaded** in atom!
    5. switch back to `feature` branch
    6. the README in atom will be still its previous version from old `deploy` branch

-- Add text below --
