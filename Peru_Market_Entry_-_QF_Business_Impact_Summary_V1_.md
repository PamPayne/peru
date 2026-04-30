---
country: Peru
document_name: Peru Market Entry - QF Business Impact Summary
source_file: Peru Market Entry - QF Business Impact Summary V1 .pdf
extracted_date: 2026-04-30
jurisdiction: Peru
---

# Peru Market Entry - QF Business Impact Summary

Created by John Crofton (ZA-DUR)

## Table of Contents

- Table of Contents
- Details
- Revision History
- Introduction
- Impact Analysis Summary
- Requirements

## Details

| Description | Detail |
|---|---|
| Document Status |  |
| Document Owner | John Crofton |
| Platform Space/Area | MIGS |
| Black Date | 14 March 2024 - GGL input along with Derivco compliance to confirm. |
| Operators | QF Ops |
| Regulator | MINCETUR - https://www.gob.pe/mincetur |
| Related Documents | Markets Workbook - v0.02 Spreadsheet |

## Revision History

| Revision | Date | Changed By | Reason |
|---|---|---|---|
| 0.01 | 30 Jan 2024 | John Crofton | v0.01 |
| 0.02 |  |  |  |

## Introduction

This document includes a high level impact analysis on Peru who wishes to regulate online gambling activity through their governing body: MINCETUR.

This document serves as a very high level consolidation of the feature requirements for QF, as well as the estimated impact analysis for the implementation of the project. These estimates have not been reviewed by technical staff, and should not be used as certainties.

### Notes and Assumptions

1. This estimate is purely for QF Operators.
2. Jackpots have not been confirmed as in-scope.
3. Live games have not been confirmed as in-scope.
4. We will not be involved in any of the reporting requirements (other than sending the required source betting data through Vanguard).
5. Operators will be utilising the Peruvian Sol as currency.
6. Remote access will be managed by the Operators.

## Impact Analysis Summary

| Definition | Symbol |
|---|---|
| **Low/No Impact (Existing Functionality)** The term "low impact" refers to the minimal effect it has on the development work. |  |
| **Medium Impact** The term "medium impact" refers to the moderate effect it has on the development work. |  |
| **High Impact** The term "high impact" refers to the significant effect it has on the development work. |  |
| **Questioned** Similar / Duplicate items (grouped by background highlights) |  |
| Different colours used to separate the different requirement groupings |  |
| Colour 1 |  |
| Colour 2 |  |

## Games

- PERGAM01) Display the Operator Authorisation Number and specific RG warning message.
- PERGAM02) Specific game theming is not permitted in Peru.
- PERGAM03) The Peruvian Sol should be available as a currency with the correct symbol. Note: There is no enforced currency (assume Ops will be using Sol / Dollar).
- PERGAM04) Games must support the Spanish language.
- PERGAM05) Games must not open on screens displaying the highest prize.
- PERGAM06) Game RTP must not be below 85%.

## Game History

- PERHIST01) Game History of 2 years must be provided to the player.
- PERHIST02) A "game memory" function must be provided that allows the player to replay or visit the results of previous play.

## Version Checking

- PERVER01) A version check must be run at least every 24 hours to verify critical assets. There is a very large scope list of critical assets.
- PERVER02) A version check must be run on the game critical files (incl. game rules and paytable) whenever a game is launched.
- PERVER03) We must track the date and changes to Help Files.
- PERVER04) We must track our game RTPs and changes to these RTPs.

## Requirements

## Games

| Ref No. | Legislation | Requirements | Questions / Comments | Impact |
|---|---|---|---|---|
| PERGAM01 | f) It has in a visible place in the remote sports betting gaming room, the authorization registration code granted by the MINCETUR, the RUC or NIT as appropriate, as well as the following warning: “Remote sports bets made in excess can cause gambling addiction”, according to the measures defined in Annex I of this Regulation. Regulations of Law No. 31557 - Article 37(f)  Both in the advertising of remote games and remote sports betting and in remote sports betting gambling halls, the Owner clearly places the phrase “Excessive remote sports betting and games can cause gambling addiction.” Regulations of Law No. 31557 - Article 56  26.14 Include on the technology platforms for online gambling and sports betting, in a way that is clearly visible and accessible, the MINCETUR authorisation, the taxpayer registration and the following warning: "Online gambling and sports betting in excess may cause compulsive gambling". LAW 31557 Online Gambling | To be confirmed if this applies to the Game Window. If it does, confirm if we would supply this or the Operator would use an overlay. If we supply, we will need to show the Operator Auth number and the correct RG warning message.  An RG warning message must be displayed.  An RG warning message must be displayed. | 1. Do these display items apply to the game screen, or are they just for lobby?  1. Assume this is the same message as Article 37?  1. Assume this is the same message as Article 37? | ? |
| PERGAM02 | The Owner, without prejudice to the provisions of the Law, is prohibited from: h) Exploit remote games or remote sports betting expressly prohibited under the Fifth Final Complementary Provision of the Law; as well as those who: 2. They are based on the commission of crimes, misdemeanors or administrative infractions; and, 3. Relate to events prohibited by current legislation. Regulations of Law No. 31557 - Article 38(h) | Specific gaming themes will not be permitted in Peru. E.g. Fireworks. | 1. Is there any specific game content we cannot show by Peruvian law / cultural standards?  1. e.g. Fireworks are prohibited in Peru - will it be problematic if a game has a firework theme? |  |
| PERGAM03 | a) The economic data information is collected automatically by the Technological Platform for remote gaming and/or remote sports betting, maintaining the integrity of the data: I. The total bets (Soles); ii. The total prize payments (Soles); b) The economic data information to be transmitted to the MINCETUR Data Center is recorded in national currency (Soles). Regulations of Law No. 31557 - Article 45  b) The credit meter can display the information in credits or in currency format (Sole, American Dollars or other currency). If the game's credit meter allows you to switch between credits and currency, this functionality should be user-friendly and easy to understand for the player. The credit meter must show unambiguously whether the information displayed is in credits or in currency. Regulations of Law No. 31557 - Section 5.3.5 | The Peruvian Sol currency / symbol should be available in our games.  Sol is one of the expected currencies. |  |  |
| PERGAM04 | The information provided through the player software must be offered in the Spanish language. When the information available to the player is provided in different languages, the following principles should apply: Regulations of Law No. 31557 - Section 3.5.9 | Our games must be available in Spanish. | 1. Is there any Operator need to provide these in eruvian Spanish? |  |
| PERGAM05 | d) When entering the game from the main menu or game selection screen, the game screen displayed by default must not correspond to the highest prize (unless it is the result of the player's last play). What is indicated is only related to the main game and not to bonuses or secondary features. Regulations of Law No. 31557 - Section 5.3.2 | Games must not open on a screen displaying the highest prize. |  |  |
| PERGAM06 | Each game must have a theoretical return of no less than eighty-five percent (85%) over the expected life of the game. Progressive jackpots, incremental jackpots, bonus prizes, etc. are not included in the payout percentage if they are external to the game, unless required for the operation. Regulations of Law No. 31557 - Section 5.7.1 | Game RTP must not be below 85%. |  |  |

## Game History

| Ref No. | Legislation | Requirements | Questions / Comments | Impact |
|---|---|---|---|---|
| PERHIST01 | The Technological Platform must have the ability to generate a record of transactions or gaming account summary history, when required by the player. The information must be available to the player for at least two (02) years, and must include at least the following types of transactions: b) Game history (by game theme); i. The name of the game theme and the type of game (reel, blackjack, poker, table, etc.); ii. Total amount wagered, including any bonus credits (if applicable); and iii. Total amount won for full games, including, any bonus credits and/or prizes, and any progressive jackpot and/or incremental progressive jackpot (if applicable). iv. Total number of cancellations. Regulations of Law No. 31557 - Section 3.4.6 | Game history of 2 years must be accessible to the player. | 1. When they reference "total" can we assume they mean the total for that round / game cycle? Or are they looking for totals over the date range specified by the player?  2. A history of 2 years may be dev work for Playcheck, assuming that is the tool we use. |  |
| PERHIST02 | A 'game memory' function is provided to the player, either as a recreation or by description. The 'game memory' function clearly indicates that it is a repetition of the previous game. Game memory must consist of graphics, text, video content, or some combination of these options, or other media, as long as a complete and accurate reconstruction of the game outcome and/or the player's actions is possible. It is allowed to display values in currency instead of credits. The game history should display the following information, as applicable: a) Date and time the game was played; b) The denomination played in the game, if it is a multiple denomination type game; c) The screen associated with the final result of the game, either graphically or through a clear textual description; d) The funds available for betting at the beginning of the game and/or at the end of the game; e) Total amount wagered, including bonus credits; f) Total amount earned, including: I. Any bonus credits and/or prizes; ii. Any progressive jackpot and/or incremental progressive jackpot; g) Any deposit of money to the non-bet game account, which has occurred between the start and the end of the game; h) The results of any player choices involved in the outcome of the game; i) The results of any intermediate game phase, such as double/risk or bonus games; j) If a progressive jackpot and/or an incremental progressive jackpot was won, an indication that the progressive jackpot was awarded; and k) Any “player advice” offered to the player for skill games. The game memory must reflect at least the last fifty (50) events of completed bonus games. If a bonus game consists of 'x number of events', each with separate results, each of the 'x events', up to fifty, must be shown with its corresponding result regardless of whether the result was a loss or a win. Regulations of Law No. 31557 - Section 5.14.1 - 5.14.3 | A "game memory" function must be introduced that allows the player to replay or revisit the results of a previous game. | 1. Would Playcheck be sufficient to cater for this? 2. If so, I don't believe steps g) and k) are catered for currently in Playcheck. |  |

## Version Checking

| Ref No. | Legislation | Requirements | Questions / Comments | Impact |
|---|---|---|---|---|
| PERVER01 | The Technological Platform must have a self-diagnosis method that, at least every 30 days, verifies and authenticates that all components of critical control programs or critical files that may affect game operations (executables, libraries, Platform configuration Technology or games, operating system files, components that control the required reports of the Technology Platform, and database elements that may affect the operations of the Technology Platform) are identical to those evaluated and approved by the Certification Laboratory authorized that carried out the corresponding technical evaluation. Regulations of Law No. 31557 - Section 3.2.1  The authentication method for control programs or files classified as critical must: a) Use a hashing algorithm that generates a 160-bit (40-digit) message digest like minimum. If other algorithms or methodologies are used, the authorized Certification Laboratory proceeds to evaluate them and authorize their use if appropriate; and b) Generate and display an authentication error message when any critical component of the control program is determined to be invalid. a) The hashing algorithm used for the verification of each component of the critical control program or critical file must meet the following requirements: I. Minimum of 160 bits (40 digits); and ii. Allow its use from a personal computer. You can also use installation media such as: USB, DVD CD or other similar media. c) For the purposes of this Regulation, the SHA-1 Algorithm is considered approved ex officio by MINCETUR as a means of verification of the control program or other components, software, applications, database model. Any other algorithm to be used for this purpose must comply with what is stated in literal a) of 3.2.2. of this Technical Standard; Regulations of Law No. 31557 - Section 3.2.1 & 3.2.2  The Technological Platform must have a self-diagnosis method, which at least every 24 hours, verifies and authenticates that all components of the critical control programs or critical files that may affect game operations (executables, libraries, Platform configuration Technology or sports betting, operating system files, components that control the required reports of the Technology Platform, and database elements that may affect the operations of the Technology Platform) are identical to those evaluated and approved by the Technology Laboratory. authorized certification that carried out the corresponding technical evaluation. Regulations of Law No. 31557 - Section 8.2.1 | There must be a version check of critical assets at least once every 30 days.  A specific algorithm must be used, and errors must be displayed.  Daily critical file validation. | 1. We can likely use Integrity Checker for this. 2. The scope of critical assets is very large, and must be defined. |  |
| PERVER02 | The player software installed on the Game Media, each time it is loaded for use, and when supported by the Technology Platform, must authenticate that all its critical components are correct. Critical software components may include, but are not limited to, game rules, paytable information, elements that control communications between the Gaming Medium and the Technology Platform, or other software components that are necessary to ensure the proper functioning of the Software. software. In the case of a failed authentication (program incompatibility or authentication failure), the software prevents game operations and displays a clear, simple and unambiguous error message. Regulations of Law No. 31557 - Section 3.5.2 | A version check needs to take place on the game critical files, including rules and paytable, whenever the game is launched. | The impact of this item can vary substantially depending on the interpretation: 1. Is this something like an Integrity Checker check per game whenever a game is launched (external tool verification of critical files)? 2. Will this be required for browser based games? Does it only apply to downloadable clients? 3. Potentially does this mean we only check when the system is first loaded, for example the check veyron does against all the games when it first loads? |  |
| PERVER03 | Rules of the game means any written, graphic, and auditory information provided to the public with regards to remote gaming operations or remote sports betting. The Owner must adopt, and adhere to, the complete game rules offered. d) The Owner must keep a record of any changes in the game rules related to the games. e) When the rules of the game are altered for the games being offered, any rule change must include a date and time stamp showing the rule applicable in each period. If multiple rules apply to a game, the Owner must apply the rules in effect when the bet was accepted. The following information must be available to the player. The functionality to display the information required in this section must be displayed by the player interface or a page accessible to the player: a) The methods of applying funds to a player's account (cash, bank transfer, money order, debit instrument, credit card, electronic funds transfer, etc.), including a clear and concise explanation of all fees (if is applicable); Regulations of Law No. 31557 - 15.1 | Must keep a record of the date and changes to game rules. | 1. Is this a process we currently follow? 2. Do we keep the bolded information in help files? |  |
| PERVER04 | The Owner must maintain accurate and updated documentation (PAR sheets) that indicate the theoretical return to player (RTP) percentages for each home banking game based on the appropriate levels of credits wagered, as well as the number of credits that can be played, the payout schedule and other information descriptive of the particular type of game. Additionally: a) Records must be maintained for each game indicating the initial Return to Player RTP percentage, the dates and type of changes made that affect the game's Return to Player RTP percentage, and the recalculation of the Return to Player RTP percentage due to the changes. b) Each change to a game's Return to Player RTP percentage, including adding and/or changing the progressive jackpot or increasing the jackpot, results in that game being treated as new for all reporting and records. Regulations of Law No. 31557 - 16.1 | Must keep records of all our games' RTPs, and record any changes to these RTPs. | 1. Who manages this list - do we provide it to the Op? 2. Do we document changes to the RTPs? |  |