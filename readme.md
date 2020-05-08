# DarkRotations Readme
#### [Environment](#Environment)
#### [Interface](#Interface)
#### [Buttons](#Buttons)
#### [Color](#Color)
#### [Interface](#Interface)
#### [Window](#Window)
#### [Rotations](#Rotations)
##### [Other](#Other)
##### [Examples](#Examples)


# Environment

## Buff
- exists()

        Check if a buff exists.
- down()

        Return true if a buff is down.
- up()

        Returns true if a buff is up.
- any()

        Return true if any buff is up.
- count

        Returns the amount of buffs that are active.
- remains

        Returns the remaning duration of the buff (in seconds).
- duration

        Returns the duration of the buff.
- stealable

        Returns true if the buff can be spellstealed.

## Cast
- Cast(spell, unit)
    
        spell:
                spell ID or name.
            
        unit:
                Unit (player, target, focus, party1, ..)
        
        example: 
                Cast(SB.Stealth);
                Cast(SB.ChaosBolt, "focus");
                Cast(SB.Conflagurate, "party1");

## Debuff
- exists()

        Check if a debuff exists.
- down()

        Return true if a debuff is down.
- up()

        Returns true if a debuff is up.
- any()

        Return true if any debuff is up.
- count

        Returns the amount of debuffs that are active.
- remains

        Returns the remaning duration of the debuff (in seconds).
- duration

        Returns the duration of the debuff.


## Enemies
- count(func)

        Returns the amount of nearby enemys.
- match(func)

        TODO
- around(distance)

        Returns the amount of nearby enemys in a given distance.

## Environment


## Group
- count(func)
- match(func)
- buffable(spell)
- removable(...)
- dispellable(spell)
- under(...)

## Health
- percent

        Returns the unit health in percentage. (0.00 ~ 100).
- actual

        Returns the actual unit health.
- effective
- incoming

        Returns the incomming (unfinished healing amount) health of the unit.
- missing

        Returns the missing health of the unit.
        
Example:

        player.acutal;      -- obtains actual player HP
        target.incoming;    -- obtains health from target player
        
## Logical
'^player',
'^pet',
'^vehicle',
'^target',
'^focus',
'^mouseover',
'^none',
'^npc',
'^party[1-4]',
'^raid[1-4]?[0-9]',
'^boss[1-5]',
'^arena[1-5]'

## Modifier
- shift
- control
- alt
- lshift
- lcontrol
- lalt
- rshift
- rcontrol
- ralt

## Power
- base
- mana
- rage
- focus
- energy
- combopoints
- runes
- runicpower
- soulshards
- lunarpower
- astral
- holypower
- maelstrom
- chi
- insanity
- arcanecharges
- fury
- pain

## Powertype
- actual
- max
- deficit
- deficitpercent
- percent
- regen
- predict
- predictpercent
- regenpercent
- tomax

## Runes
- count

## Spell
- cooldown
- exists
- castingtime
- charges
- fractionalCharges
- recharge
- lastcast
- castable
- current

## Unit
- buff
- debuff
- health
- spell
- power
- enemies
- elive
- level
- dead
- enemy
- friend
- name
- exists
- guid
- distance
- channeling(spell)
- castingpercent
- moving
- has_stealable (spellsteal)
- combat
- interrupt(%, spell)
- unit_in_range(spell)
- totem(name)
- talent(a, b)
- castable
- removable
- dispellable


## Virtual

# Interface
## Buttons
- commands
/dr move
/dr size button_size
/dr resize button_size

- button_toggle
-- master_toggle
-- cooldowns
-- interrupts
-- multitarget

## Color
- red
- dark_red
- pink
- dark_pink
- purple
- dark_purple
- indigo
- dark_indigo
- blue
- dark_blue
- cyan
- dark_cyan
- teal
- dark_teal
- green
- dark_green
- lime
- dark_lime
- yellow
- dark_yellow
- amber
- dark_amber
- orange
- dark_orange
- brown
- dark_brown
- grey
- dark_grey
- warrior_brown

## Interface
- icons (make list & tooltip name?)

## Window

# Rotation


## Rotation
## Timer

# Other

## data.data - null
## data.removables - spell ID's that need to be removed in PvE?

# Examples