Castle Crashers Access, test build 0.7.2

A screen reader mod for the Steam version of Castle Crashers. It speaks
through your screen reader using Prism, and falls back to the Windows voice if
no screen reader is found.

It reads the menus, character select, the world map, the shops and the stats
screen, and new text the game puts on screen, such as tips, prompts and
messages. In levels it has gameplay sounds: an enemy radar, wall and terrain
sounds, guidance to exits, items, chests and princesses, and spoken enemy
counts, boss health and low health.

The story has been played with the mod from Home Castle through the Cyclops'
Fortress. Past that point nothing has been checked yet: if you get further,
please send your log (see IF SOMETHING IS WRONG at the end), even when
everything went well. It shows what the mod heard and said in each level.


WHAT'S NEW IN 0.7.2

- Keyboard players hear their own keys. Hints, trainer lessons, combos, magic
  moves and the game's own tips name the key set in the game's Keyboard
  Settings ("Press S to take it", "Hold Control to block"), and controller
  players hear the controller buttons. The mod follows whichever you used
  last. A controller is not needed: everything works from the keyboard, and
  the mod's own commands are on F1 to F12.
- Keyboard Settings is read: each line says the action and its key, for
  example "Light Attack: S, 5 of 20", and the new key when you change one.
- The Controller screen (Help & Settings, Settings) reads the controller
  layout instead of nonsense.
- PlayStation controllers (DualSense, DualSense Edge, DualShock 4), with Steam
  Input on: the mod's stick commands work. The game gets these controllers
  through Steam Input, where the mod couldn't see them; it now reads them
  directly, by USB or Bluetooth.
- Play Online: after choosing the mode, "Play with anyone" and "Play with
  friends" are read (they were read as the art style question).


WHAT'S NEW IN 0.7.1

- Fixed: with the "Fresh art" look (Painter Boss Paradise), the game crashed
  as soon as the world map opened. The mod's change to the Fresh art map file
  moved the map's pictures out of place. Run Install.cmd again: it repairs
  the file. Classic art was not affected.


WHAT'S NEW IN 0.7.0

- Fixed: the game crashed when the world map opened after beating the
  Catfish, and lost the progress since the last save. Everything past Rapids
  Ride was blocked by this.
- Menus are read as soon as they open, with their title and any question
  text, for example "Paused. Resume Game, 1 of 5" or "Are You Sure? You will
  lose any unsaved progress. No, 1 of 2". Positions count only the choices
  you can move to. The art style question at start-up is read.
- Knocked into the ground: the mod now says to wiggle left and right (it used
  to say tap X, which doesn't work).
- After freeing a princess, walk into her for the kiss that ends the level;
  the mod now says so.
- The level results are read: kills, gold and experience.
- World map: paths to levels you haven't opened yet are left out, and the
  Catfish is read by name.
- Shift+F3 leaves the way back (where you came in) last, so the first press
  at the start of a level doesn't lead you out of it, and walking to an exit
  leads you right into it.
- Walking to a chest or the princess post leads you to a spot beside it
  (hits from on top of it miss).
- New hints when you're stuck on the way somewhere: gates to break, ledges
  to jump up, drop-offs to walk off (with how to get past their corner), and
  climbs such as vines and ladders. The way to a chest that runs through an
  exit is flagged before you walk out of the level.
- Gates and the big rock in Tall Grass Field (moved after eating a sandwich)
  are announced. Bosses are named: the Troll Mother, the Giant Catfish, the
  Cyclops; other bosses say what they look like, for example "Boss, a bear".
  Bats, scorpions and spiky fish are named in the enemy summary.
- The "in reach" tick works for big bosses like the War Machine, which can
  be hit from further away.
- Less chatter: enemy counts while a group trickles in, during boss fights,
  and when one enemy keeps dropping in and out; "Clear" while a boss has only
  dived or flown off; a chest announced twice; key labels such as "Tab".
- Briefings for the deer chase in the Abandoned Mill, the Catfish, the
  catapults in Flowery Field and the carriage chase in the Parade.
- Animal orbs are named properly (it said "Owlet retrieves").
- The Weapon Frog: the weapons on its rack are read. F8 steps through them
  with their stats, Shift+F3 walks you to one, and in front of one you hear
  "In front of Mace: 1 percent critical hits. Your Thin Sword: agility plus 1.
  Press X to take it." It names the weapon the game will actually give you.
- The Animal Ark: walk onto an animal to swap it for yours; the mod says which
  animal now follows you and what it does.
- Shops say each offer once, and briefings tell you what the Blacksmith, the
  Weapon Frog and the Animal Ark are.
- Arriving at an exit says "keep walking into it": the doorway takes you a
  step further than where the guide stops.


INSTALLING

1. Unzip this folder anywhere.
2. Run Install.cmd. Windows will ask for permission to change the game
   folder; choose Yes, and the installer continues in a new window. It finds Castle Crashers in your Steam libraries and tells
   you where it installed. If it cannot find the game, it asks you to type the
   folder that contains castle.exe.
3. Start the game from Steam. After a few seconds you should hear a short
   rising chime, which means gameplay sounds are working, and
   "Castle Crashers Access starting", then "Castle Crashers Access loaded. Press F1 for keys."

Updating from 0.6.6: run Install.cmd again; it replaces the old files.

To remove the mod, run Uninstall.cmd. If another mod had its own dinput8.dll
in the game folder, the installer kept a copy and Uninstall puts it back.

Map reading and gameplay sounds work by adding a few lines to your own copy
of three game files: data\game\map.pak, map_new.pak and main.pak. The
added lines report positions to the mod, and make one change to the game:
things dropped on the ground no longer vanish after about ten seconds, so
you have time to find them. The installer
keeps the originals next to them and Uninstall puts them back. If Steam updates
the game or you use Verify integrity of game files, the originals return and
these features stop; run Install.cmd again to add them back. If the game ever
fails to start after installing, run Uninstall.cmd and send the log.


WHAT SHOULD SPEAK

- Menus: the focused item when a menu opens (main menu, pause menu, Help and
  Settings and so on), then the item you move to, with its position among
  the items on screen, for example "Help and settings, 3 of 6". Options say
  their value, and the new value when you change it. Items you cannot choose
  say "unavailable". The art style question at start-up reads "Classic art"
  and "Fresh art" with what each one brings; left and right switch.
- Character select: the character you scroll to, their level, and a short
  description of how they look, for example "Red Knight, level 4. A knight in
  a gray helmet with a slit visor, wearing a red tunic. Lightning magic." When more than one player is choosing, it says which
  player, for example "Player 2, Thief, level 1".
- World map: "World map" when it opens (the first time with a short hint),
  then the level you are standing on or walking to, and whether it is
  completed or locked, for example "Barbarian War, completed". You reach the
  map by leaving a level through its exit onward. Moving between levels walks
  your character along the map's paths. The name is read as you set off, and
  a soft two-note step plays when you arrive and are standing on the level:
  only then does A play it. On arrival you also hear the paths from there,
  for example "Paths: left to Barbarian War, right to Forest Entrance or Dock,
  down to Insane Store or Home Castle." Paths to levels you haven't opened
  yet are left out, and so is a fork that leads to one (the path down from
  Home Castle opens with the Insane Store). Press F5, F7 or the left stick on the
  map to hear where you are and the paths again.
- Trainer lessons with the button named (your keyboard key when you play on
  the keyboard), using standard controller names on a controller:
  "Press X for a LIGHT ATTACK", "Hold the left trigger to BLOCK the
  baddies!", "Hold the right trigger and press Y for a SPLASH ATTACK".
  The layout is: A jump, X light attack, Y heavy attack, B use item,
  bumpers change item, left trigger block, right trigger magic.
- Items: when you get a new item for the item bar (the bow, boomerang, shovel
  and so on) you hear "New item:" and its name. F5 lists the items you have
  and which one is selected; "none yet" means you have no items to use. The
  name of the item you switch to with the bumpers, with how many
  you have of potions, bombs and sandwiches, for example "Health potions, 2".
  Picking one up says so, and using one says how many are left. Items the mod
  can't name yet are read as "Special item" and a number; tell me which ones
  you meet.
- Weapons: weapons on the ground are not picked up by walking over them. When
  you stand on one, you hear what it is, its stats and yours, for example "You
  are standing on Gold Sword: magic plus 4, defense plus 1. Your Thin Sword:
  agility plus 1. Press X to take it." Pressing X (light attack) there swaps
  it for yours, so watch for this message in a fight. If the weapon needs a
  higher level than yours, taking it only adds it to the Weapon Frog for later.
  When you take one you hear "New weapon:" with its stats. The Shift+F3 list
  gives each weapon's stats after its name. F5 includes your current weapon.
- Shops: shop items stand in the room (Castle Keep has a shop once you clear
  it; the stores on the world map work the same way). They are in the
  Shift+F3 list with their price, for example "shop: health potion, 12 gold",
  and weapons with their stats. When you stand at one you hear what it is,
  the price and your gold, for example "health potion for 12 gold. You have
  20. Press X to buy." You also hear "Not enough gold", "You already have as
  many as you can carry", and "Bought". F5 includes your gold.
- Animal orbs: in the Animal Ark and anywhere one is waiting in a level, the
  animals are in the Shift+F3 list by name, for example "Owlet, animal orb".
  Walk up to one and it starts following you: you hear its name and what it
  does, for example "Owlet is following you." followed by its description.
  The names and descriptions are the game's own, the same ones the Ark's vet
  shows. F5 includes your animal.
- Level ups: "Level up! Level 4. 2 skill points to spend on the world map",
  with a rising chime. When the level brings a new combo, its buttons and what
  it does are read too, for example "New combo: X, Y: an uppercut that
  launches the enemy into the air." Ctrl+F5 lists all the combos you have.
- The stats screen, which the world map opens by itself when you have skill
  points: points to spend and all four stats when it opens, then the stat you
  move to, each point you add or take back with the points left, and the
  "are you sure" confirmation. Up and down choose, right adds a point, left
  takes it back, A confirms.
- New text on screen: loading tips, prompts such as "Press START", and
  messages such as the art mode notice. Lines that appear together are read
  together; text the game keeps repeating is read once.
- Area and screen names when they change, for example "Home Castle",
  "Game Lobby" or "Arena Select Menu".

GAMEPLAY SOUNDS

The pitch code (the same as in ShaolinAccess): every sound that points at
something is built on one note, the A above middle C. On that note, with a
bright, buzzy sound, the thing is in your lane, level with you. Higher means it
is further up the screen, so walk up; lower means further down, so walk down.
The pitch moves one whole step per lane (about one character's width of
depth), up to an octave. Left and right are which ear the sound is in.

Each kind of thing has its own sound:
  enemies   a soft, short blip; in your lane it becomes a gentle buzz
  trainers  a two-note call
  exits     a bell that rings on
  target    a woodblock click (the thing you chose with Shift+F3)
  gold, gems        a bright metallic ting
  food              a warm, soft bloop
  weapons           a sword being drawn: a rising scrape, then the blade ringing
  the bow           a bowstring twang, then an arrow whooshing away
  potions, sandwiches and other special items  a little rising chime
  walls     a steady hum, and a knock when you bump into one

Enemy radar: about once a second, the three nearest enemies each give a soft
blip, nearest first. Far enemies are quieter. A boss gives a heavy low double
beat, like a war drum, and a mini-boss (a big enemy partway through a level,
like the War Machine) a low metal clang. An
enemy that is off the ground (climbing a ladder, jumping, or knocked into the
air) gives a blip that rises, twice, instead of a steady one: wait for it to
come down, or hit it while it's up.

Pickups: about every second, the three nearest things lying on the ground
within reach of the screen sound from where they are, using the pitch code.
You collect something by walking onto it, and you have to be very nearly in
line with it (within about half a lane), so the in-lane version of its sound
only plays when you are close enough in line to collect it. Pickups are also
in the Shift+F3 list ("gold", "food", "weapon", "health potion" and so on);
walking to one ends with "Got it" when you collect it. Things lying on a
table are named "on a table": jump up onto the table to reach them. Ctrl+F6 turns pickup
sounds on or off.

Hits (as in the Hades accessibility mods): when an enemy takes damage, a
short tone plays from where it is. Its pitch is the health the enemy has
left: high means barely scratched, low means nearly dead, so you can hear how
much each hit takes off. A low, falling thump means you killed it.

When you get hit: a low, rough crunch, unlike the clean tones of your own
hits. Its pitch is the health you have left, higher when you are healthy and
lower as you get close to going down, and it is louder for bigger hits. It
comes from the side of the enemy that most likely hit you (the nearest one
roughly in your lane). Health is spoken at each quarter: "Health 75 percent",
"Health 50 percent", and below a quarter "Health 20 percent, low!". If you
are knocked into the air you hear a falling whistle, and a heavy thud when
you land. "You're down!" means your health ran out.

Jumping and landing: a whoosh when you or an enemy leaves the ground, a thud
on landing. When an enemy goes up just after you hit it, you hear a higher,
rising whoosh instead: it has been knocked into the air, and you can keep
hitting it there. Enemy jumps and landings are quieter than yours.
Alt+F6 turns hit, jump and landing sounds on or off (including the sound
when you get hit; health is still spoken).

Items on the ground: flick the right stick right (or press F8) to step to the
next item lying around, nearest first, and left (or Shift+F8) to go back. Each
one is read with its number, for example "gold, 1 of 3, 5 steps right, in your
lane", and becomes your target, so its own sound leads you to it. After the
last one you hear "End of items". The list is made fresh if you haven't used
it for 8 seconds. Weapons drop only now and then, when an enemy carrying one
dies, or when you swap yours.

Which enemies: press the left stick button (or F7) to hear what is left,
for example "2 barbarians, 1 archer and 1 imp." Archers are thieves with
bows, who shoot down your lane from a distance.

Cannonballs: cannons like the War Machine fire at where you stand, and the
game marks the landing spot with a red crosshair. When one is fired you hear
a falling whistle from where it will land. While you are standing on the spot
(within about a lane up or down and a few steps across) a fast, urgent beep
plays: move until it stops, then you are clear of that ball.

Boss attacks: for the Barbarian Boss, the Corn Boss and the War Machine, each
attack is spoken as the boss starts it, with a short alarm from its side, for
example "Punch!", "Spikes!" or "Slam! Get away!".

Knocked into the ground or caught: some attacks pin you so you can't move
(the Barbarian Boss's shield slam buries you; some enemies grab you or lock
swords with you). You hear "Knocked into the ground! Wiggle left and right
fast to dig out" or "Caught! Tap X, Y or A fast to break free", then a double
beep every second until you are out, and "Free."

After a boss: the level doesn't end through a door. A treasure chest falls on
the beaten boss (hit it three times to open it), and a princess is tied to a
post. Hit the post: the rope takes a few seconds to cut, then you hear "The
rope is cut", and you walk into her for the kiss that ends the level. When
the last enemy is beaten, and again when each appears, you hear where it is,
and both are in the Shift+F3 list as "treasure chest" and "princess". Walking
to one leads you to a spot beside it (hits from on top of it miss) and ends
with "In reach. It's on your right: face it and press X." You don't need to
jump; the post stands against the back wall, so stand in its lane.

Results: when a level ends, the tally is read, for example "Results: 47
kills, 83 gold, 18 experience."

Gates: some ways on are shut by a gate you break (the end of Barbarian War,
a fallen pillar in Thieves' Forest). When one is near and no enemies are
left you hear "A gate blocks the way" and where; walking into it with a
Shift+F3 target says "A gate is in the way: hit it until it breaks."

Magic moves: your Magic skill unlocks new moves. When you start a level with
a new one, it is named with how to use it, for example "New magic: magic
projectile. To use it, hold the right trigger and press B." F5 lists the moves
you have and the next one to come. The moves and the Magic skill they need:
splash attack 1 (right trigger and Y), magic projectile 5 (right trigger and
B), air projectile 10 (jump, then right trigger and Y), elemental infusion 15
(X, X, X, Y), magic jump 20 (right trigger and A).

Friends: in some levels computer-controlled fighters join your side (like
the gray knight you can free in Barbarian War). When one joins you hear a
happy rising chime from its side and "A gray knight is fighting on your side",
and if it falls, "A gray knight has fallen." The enemy summary (left stick or
F7) ends with how many friends are with you.

Stuck on the way somewhere: while walking to something you picked with
Shift+F3, if you stop getting closer because something is in the way, you
hear which way gets round it, for example "Blocked. Move up a little, then
right." At an edge between two heights it says how to cross it: "A ledge. Jump
while walking right to get up it", or, at the front corner of a drop where the
cliff face blocks you, "The edge of a drop. Move up a little, then walk right
to drop down." These hints wait while enemies are close.

Archer warning: when an archer is lined up with you in your lane, a sharp
click and a falling bowstring sound come from its side, and repeat every two
seconds while you stay lined up. Step up or down a lane to get out of its
line, or run at it. Human-shaped enemies are
named by the character they look like; creatures (bees, beetles, trolls, big
trolls, fish, spiky fish, bats, scorpions, imps, slimes) by what they are. Anything the mod can't name yet
is counted as "other enemies".

In reach: a faint high tick means an enemy is lined up and close enough to
hit.

Wall hum: nearby walls hum steadily, louder the closer they are (within about
four character widths). A low hum on the left or right means a wall on that
side. A higher hum in the middle means a wall up the screen, a deeper hum in
the middle means a wall down the screen. Tables and similar obstacles count as
walls. Shift+F6 turns the hum on or off.

Walls and ground: a low knock when you walk into a wall. Other surfaces have
their own sounds: three rising notes for stairs and climbs (vines, ladders), a slide down for a ledge, a
watery sweep for water, a buzz for a hazard such as a pit, a double knock for
a raised surface like a table. A two-note chime comes from the direction of a
nearby level exit.

Walking to things: Shift+F3 (or the right stick button on a controller) picks
the nearest thing to walk to, such as a trainer or an exit, and says where it
is, for example "Walking to exit, 40 steps right, 2 lanes up". A woodblock
click then leads you there, faster as you get closer, using the pitch code.
The click follows a route around walls: it comes from the next point you can
walk to in a straight line, so if the target is behind a wall it leads you
around, for example back to a staircase and up it. The exit bell follows the
same route. When you
reach it you hear "Arrived at" and its name. Press again for the next nearest
thing, until you hear "Target cleared". Ctrl+F3 lists everything nearby.

Exits: when you clear a group of enemies, a bell rings once from the way to
the exit onward. Otherwise exits are found with Shift+F3, which names them by
where they lead, for example "exit to Animal Ark", "exit to Weapon Frog" or
"exit to the world map". The exit nearest to where you came in is called
"the way back", and comes last in the Shift+F3 list, so the first press at the
start of a level doesn't lead you out of it. Where the game doesn't say where
an exit leads, it is "the exit onward".

Trainers: when no target is chosen, the nearest trainer calls with a little
two-note sound from its direction, and stops when you are close enough to
talk to it. It uses the same up and down pitch as the radar.

Level briefings: when a level starts you hear what you will be fighting there,
for example "Barbarians attack the castle in four waves". Shift+F5 repeats it.
Enemy types come from each level's own spawn list; bosses and story from the
Castle Crashers wiki.

Scenes: when a cutscene starts, you hear a short description of what happens
where one has been written (so far the Barracks opening, both Home Castle
scenes and the War Machine's arrival in Barbarian War), or just "Scene". When it ends you hear "You have control".

Spoken: the number of enemies when a group arrives (a group that trickles in
is counted at most every 6 seconds, and not at all during a boss fight),
"Clear" when they are all beaten (not when a boss only dives or flies out of
sight), and the boss at 75, 50 and 25 percent. When a boss first appears you
hear its name ("Boss", "Mini-boss", or a name like "The War Machine"), its health
and which side it is on. Some bosses (like the big
barbarian at the end of Barbarian War) aren't marked as bosses by the game;
the mod treats any enemy with far more health than the rest as one.

KEYS

These are the mod's own keys. The game's keys are in Help & Settings,
Settings, Keyboard Settings (by default: arrows move, S light attack, D heavy
attack, A jump, G use item, Shift magic, Control block, R and T change item,
Escape pause; Enter plays a level on the world map).

F1   list the keys
F2   repeat the last thing spoken
F3   read every item in the current menu
F4   turn reading of all screen text on or off. Use this on screens that stay
     silent, like the world map; it reads any text the
     game changes on screen. It can be chatty.
Shift+F3 or right stick button  walk to the next nearest thing
Ctrl+F3  list nearby things
F5   your health, level, skill points to spend, current item, the number of
     enemies, where the nearest one is, and the nearest trainer and exit
Shift+F5  the level briefing again
Ctrl+F5   the combos you have, and the level of the next one
F7 or left stick button   which enemies are left
F8 / Shift+F8 or right stick flicked right / left   next / previous item on the ground
F6   turn gameplay sounds on or off
Shift+F6  turn the wall hum on or off
Ctrl+F6   turn pickup sounds on or off
Alt+F6    turn hit, jump and landing sounds on or off
F12  save a diagnostic of the current menus to the log


IF SOMETHING IS WRONG

The log is CastleAccess\castle_access.log inside the game folder. It is
replaced each time the game starts, so copy it before restarting. If the game
crashes, the game folder may also have a file whose name starts with
castle_17_crash: please send that too.

- Nothing at all is spoken: check that castle_access.log exists. If it does
  not, the mod did not load; make sure dinput8.dll is next to castle.exe.
- The log says the game version does not match: Castle Crashers was updated
  and the mod needs new addresses. Send the log.
- Speech works but a menu is silent or says "unlabelled item": go to that
  menu, press F12, and send the log. The dump shows how that menu is built.
- Speech uses the Windows voice instead of your screen reader: send
  CastleAccess\speech_helper.log too.


PLANNED

Attack callouts and names for more bosses, descriptions for more cutscenes,
and checking the levels past the Cyclops' Fortress with your logs.


CREDITS AND LICENCES

Speech is by Prism by Ethin Probst (Mozilla Public License 2.0). Hooking is
by MinHook by Tsuda Kageyu (BSD 2-clause). The approach builds on the
blind-accessible games list by Molitvan and the Castle Crashers modding work
of A1rPun, worstcc (castle-tools) and ethteck. Licences are in the licenses
folder. Castle Crashers is by The Behemoth; this mod is unofficial.
