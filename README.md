
# **CHANGELOG**

---

<details>
<summary><i>baleful_gaze_cockatrice.lua</i></summary>

> \- Duration down from 120 to 60 seconds. 
</details>

<details>
<summary><i>baleful_gaze_lizard.lua</i></summary>

> \- Duration down from 60 to 30 seconds.
</details>

<details>
<summary><i>healing.lua</i></summary>

> <details>
> <summary>- Healing formula rewritten so you heal the same each tick and heal for a %HP baseline.</summary>
>
>>     healHP = ( clearMindMod + max( 2 , tickCount % 2 * tickCount ) / 100 * maxHP + VIT / 4 + healHPMod
>>     healMP = ( clearMindMod + max( 2 , tickCount % 2 * tickCount ) ) / 100 * maxMP + MND / 4 + healMPMod
>
> </details>
> 
> \- Healing no longer generates enmity.
>
> \- Healing no longer reduces TP.
>
> \- Healing doesn't care about signet.
</details>

<!-- <details>
<summary><i>monk.lua</i></summary>

> \- Chakra now innately removes Silence and Paralysis in addition to its original effects.
>
> \- Chakra may now also remove Attribute Down, Gradual Petrify, Doom, and Curse with the use of Merit Points.
>
> <details>
> <summary>- Chakra healing formula rewritten so you heal for randomized %HP and %MP baseline.</summary>
> 
>>     minHP = ( ( 1 + monkLvl ) / 100 ) * VIT + 0.1 * maxHP
>>
>>     maxHP = ( ( ( 1 + monkLvl ) / 100 ) * VIT + 0.2 * maxHP + chakraJobPoint ) * chakraMod
>>
>>     minMP = ( ( 1 + monkLvl ) / 100 ) * MND + 0.1 * maxMP
>>
>>     maxMP = ( ( ( 1 + monkLvl ) / 100 ) * MND + 0.2 * maxMP + chakraJobPoint ) * chakraMod
> </details>
</details> -->

<details>
<summary><i>samurai.lua</i></summary>

> \- Logic changed to reflect cpp logic.
</details>

<details>
<summary><i>absorb_spell.lua</i></summary>

> \- Damage cap on damage displayed in the log removed.
>
> \- Overflow mechanic now works with mp and regardless of spell rank.
</details>

<details>
<summary><i>chocobo.lua</i></summary>

> \- Level requirement to rent Chocobos removed.
</details>

<details>
<summary><i>regimes.lua</i></summary>

> \- You now gain EXP from pages regardless of level.
</details>

<details>
<summary><i>chocobo_whistle.lua</i></summary>

> \- Base duration increased to 12 hours.
</details>

<details>
<summary><i>mob_controller.cpp</i></summary>

> \- Mobs will now attempt to deaggro when too far to gain enmity.
>
> \- Mobs will no longer aggro at different heights. Such as through the floor...
>
> \- Mobs will no longer aggro if they check Too Weak or Incredibly Easy Prey.
</details>

<details>
<summary><i>ability_state.cpp</i></summary>

> \- Provoke now sets the users enmity to x1.1 the highest enmity.
</details>

<details>
<summary><i>weaponskill_state.cpp</i></summary>

> \- Weaponskills have been reworked so that they consume base 1000 TP per use.
</details>

<details>
<summary><i>battleentity.cpp</i></summary>

> \- Agility now affects base speed.
> 
> \- Martial arts now effects all melee weapon types to a lesser degree as H2H.
> 
> \- You can now skill up on missed swings.
</details>

<details>
<summary><i>charentity.cpp</i></summary>

> \- You now skill up when casting magic regardless if the spell lands or not.
> 
> \- You now have a chance to skill up from each hit during a weaponskill.
</details>

<details>
<summary><i>mobentity.cpp</i></summary>

> \- All non-battlefield mobs can now deaggro.
</details>

<details>
<summary><i>petentity.cpp</i></summary>

> \- Wyvern types adjusted.
</details>

<details>
<summary><i>charutils.cpp</i></summary>

> \- Difficulty check is now based on level difference rather than potential exp awarded.
> 
> \- Exp gained cap has been removed.
> 
> \- Exp chains are now easier to start but still become more difficult to sustain.
> 
> \- Exp chain initial value is greater and scaling is slightly higher.
> 
> \- Players have access to all subjob abilities.
> 
> \- Your main job and sub job now BOTH gain and lose exp.
</details>

<details>
<summary><i>attack.cpp</i></summary>

> \- You can now skill up on misses.
</details>

<details>
<summary><i>attackround.cpp</i></summary>

> \- Hits from H2H should now count as seperate attacks?
</details>

<!-- <details>
<summary><i></i></summary>

> \- 
</details>

<details>
<summary><i></i></summary>

> \- 
</details> -->
