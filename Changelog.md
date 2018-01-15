# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/).
Date format is YYYY/MM/DD

## [5.0-xxx] - 2018-01-15 (Unreleased)
### Added
- New changelog system (yay).
- Option to roll multiple-sided dice with the roll command. 
  - Ex: `L!roll 2d20` (for two d20 dice).
- New cooldown mechanism for some commands.
- New slot machine game `L!slot`.
  - Price: 10 cookies / Jackpot: Global.
  - ![slot-game](https://image.prntscr.com/image/MXCNU4WKSyi1edmj3C_AYQ.png)
- New top/leaderboard command `L!top`.
  - Top 10 users with most cookies.
- New permission for `slot` (`CMD_SLOT`) and `top` (`CMD_LEADERBOARD`).

### Changed
- Christmas header (2017) to new high-quality one.
- Log system now uses Ansii colors that are read-able (happy now Minn?).
- `L!logs` system now uses the new profile system.
- `L!welcome` system now uses the new profile system.
- https://notfab.net/LewdBot now displays an updated list of commands.

### Fixed
- Music won't connect due to lack of resources (hopefully)
  - There's a new server available for audio processing @ Paris
- R34 (again)
- `L!logs` system (Please re-run the setup)
- `L!welcome` system (Please re-run the setup)

### Translations
- Added NOT_ENOUGH_COOKIES.
  - For when the user doesn't have enough cookies to perform an action.
- Added COOLDOWN_HIT.
  - For when the command cooldown has been hit.