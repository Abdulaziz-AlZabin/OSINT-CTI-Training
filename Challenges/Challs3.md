# 03 - The Cold Wallet Heist

**Starting point:** a huge Ethereum multisig outflow on 21 February 2025

An exchange moves ETH from cold to warm storage. Routine. The signers look at the screen, everything checks out, they approve. The money goes somewhere else.

Nobody broke the wallet. They broke what the signers *saw*. Work backwards from the outflow to whatever sat between the humans and the chain, find the infrastructure that was staged beforehand, then follow the money forward as it gets scrubbed.

Flag format: `CTI{answer}`. Times are UTC.

## Flags (10 points each)

| # | Find | Format |
|---|------|--------|
| 1 | Date of the theft | `YYYY-MM-DD` |
| 2 | Approximate ETH stolen | Nearest thousand |
| 3 | The third-party platform whose front end was tampered with, plus its web app domain | `platform,domain` |
| 4 | When forensics says the benign JavaScript was swapped | `YYYY-MM-DD HH:MM:SS` |
| 5 | The look-alike domain registered hours before the theft, and its registration time | `domain,time` |
| 6 | The payload armed itself for the next victim transaction at 2025-02-21 14:13:35. How long after the domain registration is that? | `HHh MMm SSs` |
| 7 | What the FBI calls this activity, and the date of its public notice | `name,date` |
| 8 | Two other tracking names for the same cluster | Two names |
| 9 | Two earlier exchange hacks tied to it through a shared address | Two names |
| 10 | The centralized mixer and the cross-chain bridge used on the way to Bitcoin | `mixer,bridge` |

## Bonus

- +5: From the FBI notice, find the first address that received the stolen funds and give its first hop on Etherscan.
- +5: This group is not the same as the fake-job-interview crypto crew. Explain why in two sentences.
- +10: Draw the full chain (initial compromise, staged infra, theft, laundering) with timestamps.
