# 02 - The Patient Maintainer

**Starting point:** `xz-utils 5.6.1` and an `sshd` that burns way too much CPU on login

March 2024. Somebody notices SSH logins are half a second slower than they should be and refuses to let it go. A compression library has no business touching sshd.

Behind the slowdown is roughly two years of friendly pull requests, helpful patches, and pressure on an exhausted maintainer. Nobody hacked in. They were *invited* in.

This one lives on GitHub and mailing list archives. Public data only. Trace the behavior, not the human. No digging into whoever might be behind the handle.

Flag format: `CTI{answer}`. Dates are `YYYY-MM-DD`, accepted within one day.

## Flags (10 points each)

| # | Find | Format |
|---|------|--------|
| 1 | The CVE for the backdoor | `CVE-YYYY-NNNNN` |
| 2 | The two upstream versions that carry it | `x.y.z,x.y.z` |
| 3 | Who disclosed it, where, and when | `name,list,date` |
| 4 | The GitHub handle that inserted it, and the upstream repo | `handle,owner/repo` |
| 5 | Date of that persona's very first patch to the project mailing list | Date |
| 6 | Date they opened a change to disable IFUNC in the OSS-Fuzz build | Date |
| 7 | Date they moved the project website to GitHub Pages | Date |
| 8 | The tag dates of the two bad releases | `date,date` |
| 9 | The build file that exists in release tarballs but not in the Git tree | Filename |
| 10 | One test file used to hide the payload | Filename |

## Bonus

- +5: How did a bug in `xz` get a foothold in the OpenSSH daemon on affected distros?
- +5: Name one commit-metadata signal analysts used to doubt the persona's claimed identity. Cite it.
- +10: Write the timeline from first patch to disclosure, with at least six dated events.
