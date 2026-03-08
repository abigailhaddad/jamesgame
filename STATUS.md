# Weirdmageddon Game - Status

## What Is It
A Gravity Falls tower defense game set during Weirdmageddon. Pick your character, collect materials, build defenses, craft weapons, and fight waves of enemies to protect locations in Gravity Falls. It's a single HTML file (`web/index.html`) hosted on Netlify at https://gamejames.netlify.app/

## What James Has Asked For (in order)

1. **A Gravity Falls game set in Weirdmageddon** where you collect materials to build defenses - DONE
2. **A close button for the build menu** - DONE
3. **Better animations and a pause button** - DONE
4. **Better character and enemy animations** (arms, legs, walking, etc.) - DONE
5. **Multiple areas/locations to defend** across a scrolling map - DONE
6. **Areas moved closer together** - DONE
7. **Waves attack one location at a time** instead of all at once - DONE
8. **Recruitable ally characters** (Mabel, Grunkle Stan, Wendy) - DONE
9. **A save button** - DONE
10. **Health bars on all enemies, players, and allies** - DONE
11. **A scrollable build menu and a restart button** - DONE
12. **Allies heal instead of being permanently knocked out** - DONE
13. **More enemy types** (added Henchmanians and Gideon-bots) - DONE
14. **Easy, Medium, and Hard difficulty modes** - DONE
15. **Coded title** (23-5-9-18-4-13-1-7-5-4-4-15-14 cipher) - DONE
16. **How to play instructions manual** - DONE
17. **Weapons** (Memory Gun, Wendy's Axe, Grappling Hook) - DONE
18. **More recruitable allies** (Soos, Ford, McGucket) - DONE
19. **Character selection** at game start (chosen character can't be recruited) - DONE

## Current Features

### Gameplay
- **Character select**: Choose from 7 characters before each game
- **Collect phase**: Walk around and pick up materials (wood, metal, crystal, journal pages)
- **Defend phase**: Waves of enemies attack one location at a time
- **Build menu**: Spend materials to build defenses, craft weapons, or recruit allies
- **3 locations to defend**: Water Tower, Mystery Shack, Greasy's Diner
- **Difficulty selection**: Easy / Medium / Hard on the title screen

### Characters (playable + recruitable)
- **Dipper** - the classic hero
- **Mabel** - fast fighter, costs 3 wood + 2 crystal
- **Grunkle Stan** - tough brawler, hits hard, costs 4 metal + 3 wood
- **Wendy** - fast and strong, costs 2 wood + 2 metal + 1 crystal
- **Soos** - tough handyman, slowly repairs nearby buildings, costs 3 wood + 2 metal
- **Ford** - genius inventor, high damage, costs 4 crystal + 1 journal
- **McGucket** - mad scientist, spawns turret bolts that auto-target enemies, costs 5 metal + 2 wood
- Whichever character you play as can't be recruited as an ally
- Allies patrol near their assigned location, chase nearby enemies, and heal back after being knocked down

### Weapons
- **Fists** - default, 1 damage
- **Memory Gun** - 2 damage, stuns enemies briefly, costs 5 metal + 3 crystal
- **Wendy's Axe** - 3 damage, big knockback, costs 4 wood + 4 metal
- **Grappling Hook** - 1 damage, long range, pulls enemies closer, costs 3 metal + 2 crystal + 2 wood
- Craft weapons from the build menu (+ button)

### Enemies
- **Eye-bats** - flying enemies, fast but lower HP
- **Gnomes** - ground enemies, basic
- **Henchmanians** - Bill's triangle minions, appear at wave 3+
- **Gideon-bots** - slow but tanky robots, appear at wave 5+

### Other Features
- How to play instructions on the title screen
- Coded cipher title (23-5-9-18-4-13-1-7-5-4-4-15-14)
- Save/Load game (stored in browser)
- Pause menu with Resume, Save, Load, Restart
- Mobile-friendly with touch d-pad controls
- Scrolling game world with camera following the player
- Death effects, walking animations, attack animations
- Health bars on everything
- Weapon indicator showing current equipped weapon

## Tech Details
- Everything is in one file: `web/index.html`
- Pure HTML, CSS, and JavaScript - no frameworks or libraries
- DOM-based rendering (divs and CSS animations, no canvas)
- Deployed automatically to Netlify when pushed to `main` branch
