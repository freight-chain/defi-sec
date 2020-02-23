# DeFi Threat Matrix

This work is inspired by [attack.mitre.org](https://attack.mitre.org). Please use attack for "normal" InfoSec/Dev/Sys security checklisting, this is ment to be specalized towards the unique issues brought about in blockchain/cryptocurrency applications (i.e. protocols).

## Contributing
Please fork this repo and update the "csv" file only (for now). We will update the table and [google sheet](https://docs.google.com/spreadsheets/d/1St4BXWpeZdcDaH5Z4nnODrerFAxfdZ4OuHofI-EbKGc/edit?usp=sharing) ourselves. 

## Roadmap
Organize attacks into primary categories
Organize attacks into folders with sub-folders for each attack
Organize mitigation strat. and "best practices"
Provide a list of tools, articles, and resources (i.e. an "awesome-list")
Encourage community driven feedback

## Files
Which format should files be in?
Markdown
CSV
JSON

## Tags 
Should tags for "potential" attacks or attacks that have been successful be utilized, and if so how implemented

## Repo Structure
- csv 
	.csv file containing the primary attack/potential attack planes
- documents
	.md files containing various proposed "best practices", for example [incident response plan](#) is an example of how teams should best communicate with their userbase and is based off of existing regulatory requirements
- LICENSE 
	MIT License
- README.md 
	The file you are reading right meow.

---


| **Protocol / Interaction Based** | **Blockchain Transaction Based** | **Non-Blockchain Sources** | **Blockchain Sources** | **Contract Language**                                   |
|----------------------------------|----------------------------------|----------------------------|------------------------|---------------------------------------------------------|
| Market Attacks                   | Economic Attack                  | Off\-Chain                 | On\-Chain              | Solidity                                                |
| Front\-Running                   | Front\-Running                   | Price Feed                 | Timestamp Dependence   | Integer Overflow and Underflow                          |
| Coordinated Attack               | Insufficient gas griefing        | Quote Stuffing             | Admin Key              | DoS with \(Unexpected\) revert                          |
| Liquidity Pocket                 | Token Inflation                  | Spoofing                   | Timelock               | DoS with Block Gas Limit                                |
| Quote Stuffing                   | Circulating Supply Attack        | Credential Access          | Lateral Movements      | Arithmetic Over/Under Flows                             |
| Wash Trading                     | Gas Griefing \(DoS\)             | Reentrancy                 | Multi\-Sig Keys        | Forcibly Sending Ether to a Contract                    |
| Ramping The Market               | Network Congestion \(uDoS\)      | Privilage Esclation        | Miner Cartel           | Delegatecall                                            |
| Cornering The Market             |                                  | Credential Access          | Finality               | Entropy Illusion                                        |
| Churning                         |                                  | Encryption Protections     |                        | Short Address/Parameter Attack                          |
| Flash Loans                      |                                  | Phishing                   |                        | Uninitialised Storage Pointers                          |
| Aggregated Transactions          |                                  | Unicode Exploits           |                        | Floating Points and Numerical Precision                 |
| Bulge Bracket Transactions       |                                  | API                        |                        | Right\-To\-Left\-Override control character \(U\+202E\) |
| Layering                         |                                  | DNS Attacks                |                        | Delegatecall to Untrusted Callee                        |
| Spoofing                         |                                  | Transaction Pool           | Transaction Pool       | Requirement Violation                                   |
| Order Book                       |                                  | Checksum Address           |                        | Shadowing State Variables                               |
| Market Index Calculation Attack  |                                  |                            |                        | Transaction Order Dependence                            |
| Flash Crash                      |                                  |                            |                        | Assert Violation                                        |
| Repo                             |                                  |                            |                        | Uninitialized Storage Pointer                           |
| Excessive Leverage               |                                  |                            |                        | Unprotected Ether Withdrawal                            |
| "Breaking the ""Buck"""          |                                  |                            |                        | Floating Pragma                                         |
| """Fake"" News"                  |                                  |                            |                        | Outdated Compiler Version                               |
| Nested Bot                       |                                  |                            |                        | Function Default Visibility                             |
| Audience of Bots                 |                                  |                            |                        |                                                         |
| Arb\. Exploit                    |                                  |                            |                        |                                                         |
| Slippage Exploit                 |                                  |                            |                        |                                                         |
| Safety Check Exploits            |                                  |                            |                        |                                                         |
| Circulating Supply Dump          |                                  |                            |                        |                                                         |
| Governance Cartel                |                                  |                            |                        |                                                         |
| "Flash ""Straddle"" "            |                                  |                            |                        |                                                         |
| Structuring                      |                                  |                            |                        |                                                         |

---
MIT License - Any rights or Trademarks are property of their respective owners. We Make No Claims on them whatsoever.