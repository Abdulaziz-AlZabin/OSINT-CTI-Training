# 05 - File Transfer Friday

**Starting point:** a web log line, `GET /human2.aspx`, 2023-05-30

You are reading IIS logs on a file transfer server. One request stands out: a file called `human2.aspx` that nobody remembers deploying. Someone asked it a question and it answered.

Figure out what that file is, what bug let it land, who is spraying it across hundreds of servers at once, and whether this crew has done it before. Spoiler for the vibe: they like file transfer products and they like Fridays.

Flag format: `CTI{answer}`. Dates are `YYYY-MM-DD`.

## Flags (10 points each)

| # | Find | Format |
|---|------|--------|
| 1 | The CVE being exploited | `CVE-YYYY-NNNNN` |
| 2 | The vulnerability class | Two words |
| 3 | The web shell's name | One word |
| 4 | The legitimate file `human2.aspx` is imitating | Filename |
| 5 | The date CISA says exploitation began | Date |
| 6 | The actor and its other name | `name,name` |
| 7 | With no parameters, the shell creates an admin account in the app database. Its name | Account name |
| 8 | The date CISA added the CVE to its Known Exploited Vulnerabilities catalog | Date |
| 9 | The same crew's earlier 2023 zero-day: product and CVE | `product,CVE` |
| 10 | First fixed version in the 2022.0.x line | Version |

## Bonus

- +5: From the Forescout analysis, give the order of three request paths in the log sample that shows exploitation then shell use.
- +5: Name this crew's older file-transfer-appliance campaign from late 2020.
- +10: Write a log-hunting query idea that would have caught this, in whatever language you like.
