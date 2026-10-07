# 04 - Muddy Waters

**Starting point:** a spear-phish that drops PowerShell, which then talks to its C2 over DNS

A government mailbox in Amman gets a lure. The attachment unpacks a script, the script starts whispering to a server through DNS queries. Somebody scribbles "MuddyWater" on the case and walks away.

Maybe. Or maybe it's something else dressed up to look like them. This group has leaked frameworks, shared tools, and has been caught planting false flags. Your job is to find out what is *actually* known about them, and then decide how much you are allowed to claim.

Flag format: `CTI{answer}`.

## Flags (10 points each)

| # | Find | Format |
|---|------|--------|
| 1 | The joint government advisory on this actor: ID and date | `AA##-###A,date` |
| 2 | The Iranian government body the advisory places them under | Name |
| 3 | MITRE ATT&CK group ID | `G####` |
| 4 | The backdoor in the advisory that tunnels C2 over DNS | One word |
| 5 | The malware that runs through a DLL disguised as a Google Update component | One word |
| 6 | The Python backdoor documented by UK NCSC that uses Telegram for C2 | Two words |
| 7 | Unit 42 looked at a claimed link to FIN7. Which single tool was the only overlap, and was the link strong? | `tool,yes/no` |
| 8 | The variant Talos found used against targets in Jordan | One word |
| 9 | The C2 framework whose source leaked in 2023, and the one they moved to | `old,new` |
| 10 | The ATT&CK technique ID for spear-phishing attachment delivery | `T####.###` |

## Bonus

- +5: A 2026 write-up describes a Netherlands-hosted server in a "MuddyWater-style" campaign. Give the IP and two C2 component filenames, and quote the attribution wording the researchers used.
- +5: Name two other Middle East countries named in recent targeting.
- +10: **The attribution call.** Write a short paragraph: who you think it is, how confident you are, evidence for, evidence against, at least two alternative explanations, and what would change your mind. "It's MuddyWater" with no caveats scores zero here.
