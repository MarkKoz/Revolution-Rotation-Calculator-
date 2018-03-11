# Revolution-Rotation-Calculator-
A Python command-line application for generating RuneScape ability bars for use with Revolution++.

## Getting Started
Refer the the appropriate sections for installing, configuring, and running the
program. Once it is running, follow the prompts to generate an ability bar:

```bash -
Startup Complete! Warning, the more abilities and the higher the time entered, higher wait times will be reached. A better processor will improve this speed.
Start Calculations? (Y/N) Y
```

### Requirements
#### Binaries
* [Python 3.6](https://www.python.org/downloads/) or higher

### Installation
Clone this repository to your local machine:

```bash
git clone https://github.com/MarkKoz/Revolution-Rotation-Calculator-.git
```

### Configuration
A file named `Configurations.txt`, located in `/src/` (same directory as
`calculator.py`), is used as the configuration of the program. All values are
case-insensitive.

##### Rotation Parameters
* `Adrenaline` - Initial adrenaline value. An integer in the range [0,100].
* `Gain` - The adrenaline gained after an ultimate. An integer in the range
  [0,100].
* `AttackSpeed` - The equipped weapon's
  [attack speed](http://runescape.wikia.com/wiki/Attack_speed#Weapons).
  The value is one of `slowest`, `slow`, `average`,  `fast`, or `fastest`.
* `Bleeds` - `true` if the opponent is affected by bleed effects; `false` otherwise.
* `Stuns` - `true` if the opponent is affected by stun effects; `false` otherwise.
* `Abilities` - A comma-delimited set (i.e. no duplicates) of names of
  abilities. The  set must be surrounded by square brackets.
* `Style` - The weapon's combat style. The value is a comma-delimited list
  surrounded by parenthesis. The first item is one of `magic`, `melee`, or
  `ranged`. The second item is an integer representing the weapon's handedness:
  `1` for 1-handed weapons; `2` for 2-handed weapons.
* `Time` - The duration of a cycle. Must be a number greater than 0.

##### Mode
* `units` - The units in which `Time`'s value is specified. Either `seconds` or
  `ticks`.

### Running
Run `calculator.py` to run the program:

```bash
python calculator.py
```

## Authors
* [NightShadeI](https://github.com/NightShadeI)
* [EZtouch](https://github.com/EZtouch)
* [Mark Kozlov](https://github.com/MarkKoz)

See also the list of [contributors](https://github.com/MarkKoz/Revolution-Rotation-Calculator-/graphs/contributors) who participated in this project.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
