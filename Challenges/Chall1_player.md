# 01 - Trojan in the Softphone

**Starting point:** `msboxonline[.]com`

March 2023. A signed desktop phone app updated itself two days ago. Now it calls home to a domain nobody can explain. The binary is clean on paper: valid signature, legit vendor, trusted for years.

That trust is the whole trick. Somebody got in upstream, and somebody got in upstream of *them*. Pull the thread until you reach the first domino.

Flag format: `CTI{answer}`. Case does not matter. Defang domains with `[.]`.

## Flags (10 points each)

| # | Find | Format |
|---|------|--------|
| 1 | The software product that got trojanized | Product name |
| 2 | The CVE assigned to the compromise | `CVE-YYYY-NNNNN` |
| 3 | Mandiant's cluster name for the operators | `UNC####` |
| 4 | CrowdStrike's name for the North Korean sub-group it tied to this | Two words |
| 5 | The Windows loader that persists through DLL side-loading (Mandiant's name) | One word |
| 6 | The directory where that loader reads its encrypted shellcode from | Full path |
| 7 | The macOS backdoor first called SIMPLESEA turned out to be which known family? | One word |
| 8 | The installer that started it all: filename and MD5 | `filename,md5` |
| 9 | The modular backdoor that installer dropped | One word |
| 10 | Your domain is one of four C2s. The other three | Three domains, comma separated |

## Bonus

- +5: Where were the icon files hosted that carried appended encoded data?
- +5: This case was a first for Mandiant. What was it?
- +10: Short write-up of your pivot path, from the domain back to patient zero.
