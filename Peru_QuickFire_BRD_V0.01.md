---
country: Peru
document_name: Peru QuickFire Solution
source_file: Peru QuickFire BRD V0.01.pdf
extracted_date: 2026-04-30
jurisdiction: Peru
---

# Peru QuickFire Solution

## Table of Contents

Contents

- TABLE OF CONTENTS ..................................................................................................................................................2
- REVISION HISTORY ....................................................................................................................................................3
- INTRODUCTION .........................................................................................................................................................4
- SCOPE ....................................................................................................................................................................4
- ASSUMPTIONS..........................................................................................................................................................4
- BUSINESS REQUIREMENTS ...........................................................................................................................................5

## Revision History

| Revision | Date | Changed By | Comments / Reason |
|---|---|---|---|
| 0.01 | 12 to 14 February 2024 | John Crofton | Initial Draft |
| 0.02 |  |  |  |

## Introduction

A regulated market is a country whereby online casinos cannot offer their services unless they are granted a license from that specific country’s gaming regulatory body.

This document provides the requirements for Peru. The requirements are based on the regulations specified by the Regulations of Law No. 31557 and associated regulations. The regulatory body is MINCETUR.

## Scope

As with most Quickfire solutions, the bulk of the work will be pushed to the operator. However, we are still responsible for the gaming content. This includes translations and currency support, as well as unique market requirements detailed in the business requirement section below.

## Assumptions

The following are out of scope. This decision has been made by GGL and the strategy behind this will allow us a quicker intake into the market.

1. Progressive Jackpots have not yet been confirmed in-scope.
2. Operators will be using the Peruvian Sol as currency.
3. Operators will be handling Reporting requirement.
4. Operators will be using common Spanish as their default casino language.
5. Operators will be managing remote access.
6. Some Operators may be using their own Container solutions to display items within the game, while others may be using our own Container: Titan. The below requirements assume the Operator will be using Titan.

## Business Requirements

### 1. Games

#### 1.1.
Prohibited or criminalised game themes (artwork, information) must not be present in games.

#### 1.2.
Games must not open on a screen that displays the highest prize available in that game.

#### 1.3.
Incomplete games must be completable. In cases where the game is suspended or cannot be completed by the player, the bet must be returned to the player.

#### 1.4.
If the player is inactive for 30 minutes their session must end.

#### 1.5.
In-Game Bonus Feature progress must be chosen by the player, or automatically after 2 minutes in the case there is only one option / path.

#### 1.6.
In-Game Bonus Feature must allow the player to opt-out if the bonus requires more credits from the player to continue.

#### 1.7.
The In-Game Bonus Bubble should be available to display the difference between real credits and bonus credits in the player’s balance.

#### 1.8.
Autoplay is allowed in the market.

### 2. Currency

#### 2.1.
No single currency was mandated in the legislation. The assumption is that the operators will at least be allowing the Peruvian Sol (S/) and the US Dollar ($).

#### 2.2.
Examples of Peruvian Sol with ISO Codes:

| Dialog Text | Symbol | Currency Code (ISO 4217) | Country Code (ISO alpha-3) |
|---|---|---|---|
| Total Wagered | S/ | PEN | PER |
| Total Payout | S/ | PEN | PER |
| Balance | S/ | PEN | PER |
| View Pays – Credits | S/ | PEN | PER |
| Bet | S/ | PEN | PER |

### 3. Languages

#### 3.1.
All our offered products must be at least available in the Spanish language.

### 4. Bet Settings

#### 4.1.
There are no specific market bet settings applicable for Peru.

#### 4.2.
The regulations do require bet limits to be available to the player. However, this will be the responsibility of the operator for Quickfire.

### 5. Help Files

#### 5.1.
Helpfiles must be made available for all our games in Spanish.

#### 5.2.
The RTP must be displayed in the Helpfiles.

#### 5.3.
Any change to the Help Files must be versioned and recorded.

### 6. Game History (Playcheck)

#### 6.1.
The operator must offer the player a transaction report for the consultation of the wins and losses with timestamps for each game event, as well as the account balances. The unique paylines or images displaying the result of each bet must be available.

#### 6.2.
Game History must be available on request by the player with up to 2 years history (2 years does not have to be immediately accessible on Playcheck).

### 7. Operational

#### 7.1.
Bonus is allowed.

#### 7.2.
Free Games is allowed.

#### 7.3.
Practice and Demo play are NOT allowed.

### 8. Return to Player (RTP)

#### 8.1.
The games operated online shall present a minimum return to the player of 85%.

#### 8.2.
A record of changes to RTP must be versioned and recorded.

### 9. Critical Files Validation (Integrity Checker)

#### 9.1.
A mechanism for verifying critical files must be available in the market, and it must perform a check on these files at least once every 24 hours.

#### 9.2.
Critical files will include game files and any platform files that have an impact on game outcomes or operations. The example included in the regulations:

(executables, libraries, Platform configuration Technology or sports betting, operating system files, components that control the required reports of the Technology Platform, and database elements that may affect the operations of the Technology Platform).

#### 9.3.
A 160-bit algorithm must be in use.

### 10. Data Retention

#### 10.1.
Data retention is required for a period of 5 years. When an account is closed, data must be stored for 5 years.

#### 10.2.
We will be required to store game history data. The personal data of customers will be the responsibility of the operator.

### 11. Remote Access

#### 11.1.
Operators must be notified if we change our infrastructure or RNG, to allow them to notify the regulator.

#### 11.2.
Operator remote access must be managed should they request access to our systems for auditing or review purposes.