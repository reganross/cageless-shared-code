# Cart Escort Harvesting Minigame

## Overview

The Cart Escort minigame is a **team-based, skill-driven activity** designed for multiple harvesting professions: Mining, Woodcutting, Masonry, Tanning, and Harvesting.  
Players escort a central cart along a path while interacting with resource nodes, fighting enemies, and managing hazards.  
The game combines **resource collection, combat, repair, XP progression, and strategic drafting** to create a high-stakes, replayable experience.

---

## Core Gameplay Loop

1. **Escort a Cart** along a predefined path.
2. **Interact with Resource Nodes**:
   - Mining: ore veins, crystals  
   - Woodcutting: trees, logs  
   - Masonry: stone blocks, rubble  
   - Tanning: animal carcasses, hides  
   - Harvesting: crops, herbs, fibers
3. **Combat & Hazard Management**:
   - Enemies attack the cart and players  
   - Environmental hazards (falling rocks, unstable terrain) appear
4. **Earn XP for Actions**:
   - XP is tracked **per mission** for the relevant harvesting skill
   - Minimum XP is required to qualify for end-of-run rewards
5. **Manage Cart Health**:
   - Cart takes damage from attacks and hazards  
   - Item drop chance is calculated based on **pre-hit HP**
   - Repairs are possible, but risk item loss if interrupted
6. **End-of-Run Draft**:
   - Shared cart inventory is distributed via the **picks-surrender draft system**  
   - Tie-breakers resolved with currency bids or random rolls

---

## XP System

Each action in the minigame grants **skill-specific XP**:

| Skill        | Example Actions                                 |
|--------------|------------------------------------------------|
| Mining       | Extract ore nodes                               |
| Woodcutting  | Chop trees, gather logs                         |
| Masonry      | Break stone blocks, collect bricks              |
| Tanning      | Skin animals, process hides                     |
| Harvesting   | Collect crops, herbs, fibers                    |

### Minimum Contribution Requirement

- Players must earn a **minimum XP threshold** in the relevant skill to qualify for rewards.  
- XP earned includes contributions from **combat, support, or repair actions** if they impact mission success.  

**Example**: Mining mission, minimum XP = 100  
- Player earns 85 XP → does not qualify  
- Player earns 120 XP → qualifies for draft

---

## Cart Health & Damage Mechanics

- Each cart has **maximum HP**.  
- Attacks reduce HP and can **cause item drops**.  

### Pre-Hit Item Loss

- Item drop chance is calculated based on **cart HP immediately before each hit**:

| Pre-Hit HP      | Item Drop Chance |
|-----------------|----------------|
| 75–100%         | 0%             |
| 50–74%          | 10–20%         |
| 25–49%          | 30–50%         |
| 1–24%           | 70–90%         |
| 0% (destroyed)  | Minigame ends; no items rewarded |

**Example Formula**:
Item Drop Chance = BaseChance × (1 - (PreHitHP / MaxHP))


- BaseChance is the inherent risk per attack.  
- Big hits on a full HP cart **do not drop items**.  

### Repairs

- Players can repair the cart to restore HP and reduce future item drop chance.  
- Repairs may **still risk item loss** if interrupted by attacks.  
- Skills or tools may improve repair efficiency or speed.

### Cart Destruction

- If HP reaches 0:
  - **Minigame ends immediately**
  - **Material rewards are lost**
  - **XP is retained**

---

## Resource Nodes & Modifiers

- Nodes along the path can be harvested for materials.  
- Each node has **modifiers** affecting yield or quality.  
- Players **see known modifiers**; unknown modifiers display as “?” until the mission is complete.  
- Cart inventory has **limited space**, scaling with:
  - Player skills
  - Number of players

---

## End-of-Run Draft: Picks-Surrender System

### Draft Mechanics

1. **Qualified players** (meeting minimum XP) submit a sealed bid:  
   > “How many picks am I willing to surrender for priority?”  
2. Draft order is highest surrender → lowest surrender.  
3. Players may only pick **up to the number of picks not surrendered**.  

### Example

Cart inventory: 12 items  
Players: 4  

| Player | Picks Surrendered |
|--------|------------------|
| A      | 2                |
| B      | 1                |
| C      | 0                |
| D      | 1                |

Draft order: A → B → D → C

### Tie Resolution

1. Optional **currency bid** (paid to other players)  
2. Random roll if still tied  

### Strategic Implications

- Trade **quantity for quality**  
- Incentivizes **knowledgeable players** to bid for high-value items  
- Adds **economic and social tension**  

---

## Activity-Specific Variations

While the **core gameplay loop is consistent**, each skill features **unique scenery, enemies, and node visuals**:

| Skill        | Environment / Scenery           | Enemy Types                | Node Appearance         |
|--------------|--------------------------------|----------------------------|------------------------|
| Mining       | Underground mines, cliffs      | Rock elementals, cave beasts | Ore veins, crystals    |
| Woodcutting  | Forests, groves                | Wolves, forest spirits    | Trees, logs            |
| Masonry      | Quarries, stone walls          | Stone golems, bandits     | Stone blocks, rubble   |
| Tanning      | Grasslands, animal pens        | Predators, rival hunters  | Animal carcasses, hides|
| Harvesting   | Fields, gardens, herbal groves | Pests, magical creatures  | Crops, herbs, fibers   |

### Optional Enhancements

- **Hybrid Missions**: Combine multiple harvesting skills.  
- **Themed Node Modifiers**: Unique to skill type.  
- **Dynamic Enemy Scaling**: Keeps tension consistent.  

---

## Summary

The Cart Escort minigame combines:

- **Core mechanics** consistent across all harvesting skills  
- **Mission-specific XP** tracking with minimum contribution thresholds  
- **Cart health & item loss** system based on pre-hit HP  
- **Repair mechanics** with risk/reward decisions  
- **Shared inventory draft** using picks-surrender system  
- **Flavorful environments and enemies** per skill  

This structure ensures **skill-driven progression, team cooperation, and high-stakes tension**, while remaining flexible and replayable across all harvesting activities.