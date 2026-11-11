# A public Linux learning method — privacy-safe summary

In less than one year of using AI, daily technical questions gradually became structured procedures. This file is an educational summary of the method, not a copy of private equipment settings.

The recurring cycle is **observe → hypothesize → inspect safely → change one thing → verify → document → hand over**.

For every technical note, record the observed symptom, a reproducible non-destructive check, why a proposed change was chosen, how the result was validated, what remains untested, and how to roll back.

For example, when one browser fails to play video while another works, investigate user-session audio services before assuming a network failure. **systemctl --user is-active pipewire pipewire-pulse wireplumber** inspects the relevant services. A restart is only appropriate when the evidence points there; it is not a universal fix.

For backups, distinguish **file copied**, **checksum verified**, and **content restored and read**. For Git, inspect **git status --short** and **git diff --check** before committing changes. An observed failure is a valuable documented result, not a reason to pretend the task passed.

**Privacy boundary:** no hostnames, network addresses, credentials, private paths, remote-access configuration or unpublished infrastructure topology are included.

The detailed public guide is in [French](GRAND_MANUEL_LINUX_PUBLIC_FR.md). © Laurent B. 2026.
