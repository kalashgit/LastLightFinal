# Last Light mechanics library — AI entry point

This directory is a documentation-only design library, excluded from Godot import by `docs/.gdignore`. The 25 supplied references are in [source/](source/00_README.md). These are concise design summaries, not complete engineering specifications or proof of implementation. Referenced scripts, JSON, wireframes, tables and formulas may not actually be supplied. Never fabricate their contents.

## Reading order and dependencies

Read root AGENTS.md and the existing roadmap first. Use the following groups to find the relevant source before changing code. Numbers refer to the source documents below.

| Domain | References | Proposed dependency |
|---|---|---|
| World, clock, persistence, sandbox | 01, 09, 14, 15 | Foundational |
| Character, XP, traits | 02, 16 | State and data model |
| Health, nutrition, weather | 03, 18, 20 | Clock, character, persistence |
| Movement, stealth, zombie AI | 04, 15, 20 | World, player state, sound |
| Combat and armor | 05, 17, 24, 25 | Movement, health, inventory |
| Inventory, crafting, loot | 06, 14, 15, 19 | Ownership and persistence |
| Character art, clothing | 11, 12, 13 | Inventory/equip state, rendering |
| Base, utilities, vehicles | 07, 10, 19 | World, crafting, persistence |
| NPC, factions, trading | 08 | Inventory, AI, world |
| Audio and sound perception | 21, 22, 23 | World and event system |

## Source index
- [Last Light — Part 1: Game Identity, Isometric Camera, Time & World Persistence](source/01_Part_1_Game_Identity_Isometric_Camera_Time_World_Persistence.md)
- [Last Light — Part 2: Character Creation, Point-Buy Traits, Occupations & 0–10 Skill Progression](source/02_Part_2_Character_Creation_Traits_Occupations_Skills.md)
- [Last Light — Part 3: Body, Moodles, Medical Trauma, Nutrition & Infection Rules](source/03_Part_3_Body_Moodles_Medical_Trauma_Nutrition_Infection.md)
- [Last Light — Part 4: Movement, Stealth, Sensory Perception, Zombie AI & Hordes](source/04_Part_4_Movement_Stealth_Sensory_Perception_Zombie_AI_Hordes.md)
- [Last Light — Part 5: Melee Combat, Firearms, Weapon Durability & Layered Armor/Tailoring](source/05_Part_5_Melee_Combat_Firearms_Durability_Layered_Armor.md)
- [Last Light — Part 6: Inventory, Physical Ownership, Containers, Crafting, Dismantling & Workstations](source/06_Part_6_Inventory_Physical_Ownership_Containers_Crafting_Workstations.md)
- [Last Light — Part 7: Base Building, Fortifications, Utilities, Farming/Livestock & Vehicles](source/07_Part_7_Base_Building_Fortifications_Utilities_Farming_Vehicles.md)
- [Last Light — Part 8: NPC Survivors, Factions, Quests, Trading & iOS Touch UI/UX Wireframes](source/08_Part_8_NPC_Survivors_Factions_Quests_Trading_iOS_UX.md)
- [Last Light — Master Sandbox Configuration & Engine Data Tables (Parts 1–8)](source/09_Master_Sandbox_Configuration_and_Engine_Data_Tables.md)
- [Last Light — Vehicles, Generators, Power Loops & Visual Vehicle Design](source/10_Vehicles_Generators_Power_Loops_Visual_Design.md)
- [Last Light — Character Modeling, Game-Ready Assets, Animations & Asset Interactions](source/11_Character_Modeling_Assets_Animations_Interactions.md)
- [Last Light — Layered Character & Paper-Doll Clothing System (Precise Specification)](source/12_Layered_Character_Paper_Doll_Clothing_Precise_Spec.md)
- [Last Light — Layered Character & Paper-Doll Clothing System](source/13_Layered_Character_Paper_Doll_Clothing_System.md)
- [Last Light — Mobile UI/HUD Design, Weight/Encumbrance & Save/Persistence Architecture](source/14_Mobile_UI_HUD_Weight_Encumbrance_Save_Persistence.md)
- [Last Light — World Loot, Containers, Zombies, Hordes & Sandbox Systems](source/15_World_Loot_Containers_Zombies_Hordes_Sandbox.md)
- [Last Light — Skills, Traits, XP & Progression Systems](source/16_Skills_Traits_XP_Progression_Systems.md)
- [Last Light — Weapon Durability, Firearms & Ballistics Systems](source/17_Weapon_Durability_Firearms_Ballistics_Systems.md)
- [Last Light — Weather, Temperature & Survival Loops](source/18_Weather_Temperature_Survival_Loops.md)
- [Last Light — Base-Building, Barricades & Crafting Systems](source/19_Base_Building_Barricades_Crafting_Systems.md)
- [Last Light — Enemy AI Sensory Detection & Health Moodle Systems](source/20_Enemy_AI_Sensory_Detection_Health_Moodle_Systems.md)
- [Last Light — Footsteps & Surface Material Synthesis Script](source/21_Footsteps_Surface_Material_Synthesis_Script.md)
- [Last Light — Procedural SFX Generator, Sound Radius Table & Repo Architecture](source/22_Procedural_SFX_Generator_Sound_Radius_Repo_Architecture.md)
- [Last Light — FMOD Audio, Sound Radius & SFX Pipeline](source/23_Project_Zomboid_FMOD_Audio_Sound_Radius_Mechanics.md)
- [Last Light Combat & Battle Mechanics Reference](source/24_Last_Light_Combat_and_Battle_Mechanics.md)
- [Last Light — Combat & Melee Mechanics Reference](source/25_Combat_and_Melee_Mechanics_Reference.md)

Read [IMPLEMENTATION.md](IMPLEMENTATION.md) for the engineering workflow. The dependency suggestions are planning guidance, not founder-approved changes to the existing roadmap.
