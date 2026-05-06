======================================================================
URGE – Ultimate Resource Grabber and Extender  v3.0.0
HOI4 Mod  ·  1.14.x  ·  Map-Screen Panel (NO decisions panel)
======================================================================

INSTALLATION
────────────
1. Place URGE.mod + URGE/ folder in:
   Windows: %USERPROFILE%\Documents\Paradox Interactive\Hearts of Iron IV\mod\
2. Enable "URGE" in the Paradox Launcher.
3. Start a new game.

HOW TO USE
──────────
• A small ⚡ button appears at the CENTER-RIGHT of your screen.
• Click it (or press B) to open/close the URGE panel.
• The panel expands to the LEFT, showing six action buttons.
• Pressing B toggles the Supremacy button (Activate or Deactivate,
  whichever is contextually appropriate).

PANEL BUTTONS
─────────────
1. Activate / Deactivate Military Supremacy  [B keybind]
   Grants the URGE Military Supremacy national spirit:
     – All attrition eliminated (heat, winter, terrain, supply)
     – All leaders → Supreme Commander trait (+976 command limit)
     – Air superiority advantage maxed
     – Naval invasion supremacy bypassed (engine defines)
     – +9,999 political power  +9,999 convoys
     NOTE: Does NOT grant stability, war support, or manpower.
   Press again to remove the spirit.

2. Summon Grand Fleet & Air Corps
   – All key technologies researched
   – Division templates: URGE Elite Infantry, URGE Armoured
     Spearhead, URGE Marine Raiders
   – 10 divisions spawned at capital (fully equipped)
   – Full ship + aircraft stockpiles of every type
   – Admirals (×3), Air Marshals (×2), Field Marshal (×1),
     Generals (×3) — all at maximum skill with URGE traits

3. Commission the Shadow Bureau  [La Résistance DLC]
   – Calls create_intelligence_agency — native naming/emblem dialog
   – 9,999 agency experience granted immediately

4. Maximize Intelligence Agency  [La Résistance DLC]
   – Unlocks all vanilla agency branches
   – 9,999 additional experience

5. Emergency Resupply
   – Fuel 100% · 9,999 convoys · 1M manpower · 9,999 PP
   – Max stability & war support · Full strategic resources

6. Commandeer National Resources
   – Capital: 10× factories, dockyards, air bases, naval bases,
     radar, fuel silos, rocket sites, nuclear reactor
   – 50 nuclear bombs · Full strategic resources
   – All key technologies re-researched

ENGINE-LEVEL BYPASSES (always active)
──────────────────────────────────────
  NNavy.NAVAL_SUPREMACY_CAN_INVADE    = -1.0  (no superiority needed)
  NNavy.AMPHIBIOUS_LANDING_PENALTY    = 0.0   (no landing penalty)
  NNavy.NAVAL_INVASION_PREPARE_HOURS  = 1     (instant prep)
  NNavy.PARADROP_AIR_SUPERIORITY_RATIO= 0.0   (no air sup for drops)
  NMilitary.FIELD_MARSHAL_ARMIES_CAP  = 1000  (1000 army groups)

TROUBLESHOOTING – PANEL NOT VISIBLE
────────────────────────────────────
If the ⚡ button does not appear after starting a new game,
check the error.log at:
  Documents\Paradox Interactive\Hearts of Iron IV\logs\error.log

The panel attaches to HOI4's internal "realmapview" window via
player_context scripted_gui. If your game version renamed that
window, open URGE/common/scripted_gui/URGE_scripted_gui.txt and
change  parent_window_name = "realmapview"  to the correct name.
You can find the window name by searching your HOI4 install's
interface/ folder for the main GUI .gui file.

COMPATIBILITY
─────────────
All URGE files use unique "URGE_" prefixes. No vanilla files are
modified. AI is excluded from all effects. Compatible with any
mod that doesn't overwrite the specific files listed above.
======================================================================
