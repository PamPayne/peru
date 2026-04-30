---
country: Peru
document_name: Peru Operator Guidelines Regulated Market Casino Compliance
source_file: QF Peru - GGL Casino - Operator Guidelines v1.0 - 22 Feb 2024.pdf
extracted_date: 2026-04-30
jurisdiction: Peru
---

# Peru Operator Guidelines

**Regulated Market Casino**  
**Compliance**

Release Date: 22nd February 2024  
Document No: 000 - 000  
Version: 1.0

## Contents

- Market Overview ............................................................................................................................................... 2
- Introduction ...................................................................................................................................................... 2
- Domain .............................................................................................................................................................. 4
- Registration ....................................................................................................................................................... 4
- Currency ............................................................................................................................................................ 4
- Languages .......................................................................................................................................................... 4
- Bonuses ............................................................................................................................................................. 4
- Practice & Demo Play ........................................................................................................................................ 5
- Account Inactivity.............................................................................................................................................. 5
- Player Protection............................................................................................................................................... 5
- Player Balance ................................................................................................................................................... 5
- Playcheck........................................................................................................................................................... 5
- Integrity Checker ............................................................................................................................................... 5
- Games ................................................................................................................................................................ 6
- Incomplete Games ............................................................................................................................................ 6
- Incomplete Games Sweeper ............................................................................................................................. 8
- Responsible Gaming ......................................................................................................................................... 8
- Data, Reporting and Access ............................................................................................................................... 9

## Market Overview

### Introduction

This document provides an overview for Games Global Limited Casino operators to comply with the regulations defined in the legislation for Peru, as provisioned by the current regulator: MINCETUR.

It defines the split in responsibilities around managing players and games in the Peruvian market, identifies what Games Global Limited will provide you with to satisfy the requirements and assists you in ensuring that the correct integrations are done to satisfy the market demands.

## Games Global Limited Solution

The following table summarises the areas and where the responsibilities lie. These responsibilities are defined since Games Global Limited is not your primary platform and does not contain all the information necessary to manage certain aspects of your players’ life cycle.

| Component | Sub-Component | Operator | GGL |
|---|---|---:|---:|
| General | Player Verification Services | Yes | No |
| General | Integration – Platform | Yes | No |
| General | Client Legislative Changes | Yes | Yes |
| General | Platform Certification | Yes | No |
| General | License Application and Submission | Yes | Yes |
| General | Practice & Demo Play | Yes | Yes |
| External Integrations | MINCETUR Exclusion Register | Yes | No |
| Login | Login & Password | Yes | No |
| Login | Online Registration | Yes | No |
| Login | Player Account Management | Yes | No |
| Login | Account Status | Yes | No |
| Login | Languages & Currency | Yes | Yes |
| Login | Terms & Conditions & Privacy Policy | Yes | No |
| Lobby | Player Balance | Yes | No |
| Lobby | Session Inactivity | Yes | No |
| Lobby | Player Protection Content | Yes | No |
| Lobby | Responsible Gaming (including deposit limits, bet limits, self- exclusions, and time-outs) | Yes | No |
| Lobby | Playcheck | Yes | Yes |
| Gaming | Game certification | Yes | Yes |
| Gaming | RNG Certification | Yes | Yes |
| Gaming | Game Rules | Yes | Yes |
| Gaming | Display Game Rules | Yes | Yes |
| Gaming | Display Game Help | Yes | Yes |
| Gaming | Display RTP | Yes | Yes |
| Back Office | Account Migration | Yes | No |
| Back Office | Game Management | Yes | Yes |
| Back Office | Account Management | Yes | No |
| Back Office | Value Adds | Yes | No |
| Back Office | Banking | Yes | No |
| Back Office | Deposit | Yes | No |
| Back Office | Withdrawals | Yes | No |

### Domain

Please ensure that your websites providing online games in this market have a Peru domain (e.g. “bet.pe”).

### Registration

As our system does not have any visibility into your registration process, you would need to manage this aspect as well as the document verification and account activation requirements for your players.

Please ensure that a player is not able to have more than one account registered on your casino and is over the age of 18 years.

If the player is detected on the MINCETUR external exclusion register, that player’s registration should be discarded.

To complete the player registration process please ensure the player agrees to your T&C’s and privacy policy which must be recorded on your platform.

### Currency

To meet regulatory requirements, the Peruvian Sol is the default currency for wagers when participating in games. The S/ symbol shall be used to represent the Peruvian Sol.

### Languages

All Game rules and Help files will be provided in Spanish by Games Global Limited.

### Bonuses

Bonus offers are allowed and may be offered to a player registered on your casino.

### Practice & Demo Play

Practice & Demo play must not be offered to unregistered players.

### Account Inactivity

After a maximum of 30 minutes of inactivity, the player's session must be disconnected. The player should be notified that their session is terminated.

### Player Protection

Player protection information must be always accessible to players on the casino website. The content on Player Protection assists players in gaming responsibly. Since you manage the lobby for your casino, please ensure that you provide players with the following info:

- Information on how gambling may be harmful.
- Information on opportunities for self-control, game restrictions and suspensions.
- Information that no minor is permitted to play.
- Information for the player to contact the Operator regarding claims or disputes.
- Information about MINCETUR with links to their website that support responsible gaming (i.e. counselling centres, treat addiction).

### Player Balance

As Games Global Limited is not your primary platform and player accounts are owned by yourselves, you would be required to continually show the player’s balance, in Peruvian currency, during the entire time the player has logged into the system. It should be possible to view the split between real and bonus credits or currency.

Players must have access to information related to their gaming activity including all transactions which modify the player’s balance.

### Playcheck

We will provide a minimum of 30 days’ worth of detailed game transaction history. The regulations specify that 2 years data must be available to the player, but this can be delivered upon request.

### Integrity Checker

We will manage a daily (24-hour) integrity verification of critical game files provided by Games Global Limited. This can be reviewed, via supplied credentials, on a web portal which will allow you to see the pass / fail results of each file.

## Games

The following game changes will be implemented by Games Global Limited and included in Peru casinos:

- Autoplay
  - AutoPlay will be available for players.
  - The player will be able to stop AutoPlay at any given moment, if enabled.
  - A maximum of 100 automatic spins will be implemented.
- Players Balance
  - The screen must show the player’s current balance, in Peruvian currency, as well as the individual bets placed.
- Help Files and Game Rules
  - We shall display the RTP in all help files.
  - Game rules, including paytables, shall always be available to players.
- Playcheck
  - Playcheck must provide data on gaming transactions for a minimum duration of 30 days.

### Incomplete Games

As Games Global Limited is not your primary platform and player accounts are owned by yourselves and multiple vendor’s games are offered, we would require you to retrieve any incomplete Games Global Limited game information for players using the Get Incomplete Games API method.

Incomplete Games feature is required for Peru. You would need to complete any development required for the user interface, translations, and game redirection. Funds must be returned to the player for any incomplete game that is cancelled by the operator. Incomplete games must be completed before the player can play the same game again. A valid operator token must be provided in the Authorization header, this can be requested via your Account Manager.

The following request call with mandatory fields needs to be made:

#### Request Call

GET /balances/product/productId/user/userId/incompleteGames

#### Required Fields

| Name | Type | Format |
|---|---|---|
| productId The ProductId (previously called CasinoId or ServerId). This identifies the system where the account is held and can be either a SessionProductId or RegisteredProductId | Integer | int32 |
| userId The UserId of the account. | Integer | int32 |

After a request call is initiated, a response will be sent back that will either be a successful or an unsuccessful (error) attempt. If successful, the below information is displayed:

#### Responses

| Name | Type | Format |
|---|---|---|
| clientId The ClientId for the game. | Integer | int32 |
| moduleId The ModuleId for the game. | Integer | int32 |
| gameName The name of the game, e.g. HTML5 - Feature Slot - Avalon. | String | int32 |
| moduleName The name of the module, e.g. Feature Slot - Avalon. | String | int32 |
| payouts The combined amount owed to the user, e.g. a payout from a win in a game. | Number | Decimal |
| sessionId SessionId allocated for the session. | Integer | int32 |
| userTransNumber The UserTransNumber is the associated user transaction number for the incomplete game. | Integer | int32 |
| wagers The combined amount taken from the user, e.g. a bet taken during a game. | Number | Decimal |

The /accounts/CheckUserExists API method returns the UserId of the player. You can use this method to retrieve the UserId to do the Incomplete games call.

#### Responses

| Name | Type | Format |
|---|---|---|
| doesExist Indicates whether the specified Username exists or not. | Boolean | int32 |
| registeredProductId The ProductId (previously called CasinoId or ServerId) against which the account was created. Only returned if the specified Username already exists. | Integer | int32 |
| suggestedUsernames Array of suggested alternate Usernames that are currently available. They are based on the provided username. Only returned if the specified Username already exists. | String |  |
| userId The UserID for the account if the Username already exists. | Integer | int32 |

### Incomplete Games Sweeper

We have implemented an Incomplete Games Sweeper.

This will run as a SQL job (FundsInPlayGameSweeper) once a day and will be used to sweep any incomplete game rounds older than 90 days.

If a player leaves a bet open for more than 90 days, the sweeper job will close the open round.

The job is based on two CasinoID level settings:

**FundsInPlay - Is Sweeper Enabled:** Used to determine whether the sweeper should even be used for this serverid.

**FundsInPlay - InActivity period in days:** Used to determine the threshold for how old a game round needs to be before sweeping it.

Note:

You are required to advise your players regarding this on your Terms and Conditions page.

### Responsible Gaming

Responsible gaming measures need to be in place to ensure that all players play responsibly and are in control of managing their gaming activity. Since our operators own the player accounts and manage their own lobby, you must ensure that the following responsible gaming options are accessible to your players:

- Deposit Limits
  - The player must have an option to set Deposit Limits. In cases where the player tries to increase (make less strict) these limits, a 24-hour cooldown must apply before the new values are implemented.
  - In the event of reaching the deposit limit, the user shall not be able to deposit further funds.
- Bet Limits
  - The player must have an option to set Bet limits. In cases where the player tries to increase (make less strict) these limits, a 24-hour cooldown must apply before the new values are implemented.
  - In the event of reaching the bet limit, the user shall not be able to start another game process.
- Self-Exclusions
  - An internal exclusion system must exist that allows the player to self-exclude either temporarily or permanently.
  - Players who self-exclude cannot login, participate in games or deposit.

- Error Codes
  - To enable the Games Global Limited system to display informative error messages to players, we require that the following error codes are returned under the prescribed conditions.

| Code | Description |
|---|---|
| 6102 | Account is locked. |
| 6104 | Player is self-excluded. |
| 6109 | Self-exclusion is over, and the player must contact the operator to lift the exclusion. The cooling period is effective once this is done. |
| 6110 | Self-exclusion is over, but the player is in the cooling period. |
| 6112 | Player is deactivated. |
| 6113 | Player is self-excluded on registry |
| 6503 | Player has insufficient funds. |
| 6505 | The player exceeded their daily protection limit. |
| 6506 | The player exceeded their weekly protection limit. |
| 6507 | The player exceeded their monthly protection limit. |
| 6508 | The player exceeded their game play duration. |
| 6509 | The player exceeded their loss limit. |
| 6510 | The player is not permitted to play this game. |
| 6114 | The player has exceeded their daily login duration limit. |
| 6115 | The player has exceeded their weekly login duration limit. |
| 6116 | The player has exceeded their monthly login duration limit. |

### Data, Reporting and Access

As Games Global Limited is not your primary platform and multiple vendor’s games are offered, please ensure that you have an acceptable environment, to:

a) enable the regulator to access, monitor and supervise any of the components of the technical gaming platform,

b) control game security and transparency,

c) provide reports as required by the regulator.

Please ensure data is kept for a minimum of 5 years.