# 🧠 Phantom Trigger Plugin - Backend TODO

---

## 📦 Core Architecture

- [ ] Create base package structure (`systems`, `managers`, `data`, `utils`)
- [ ] Define clear interfaces between systems
- [ ] Create central access point (e.g. ServiceRegistry or static managers)

---

## 👤 Player Data System

- [ ] Create PlayerData class
    - [ ] UUID
    - [ ] Selected weapon
    - [ ] Selected ability
    - [ ] Current cooldowns
    - [ ] Stats (kills, deaths)

- [ ] Create PlayerDataManager
    - [ ] Load data on join
    - [ ] Save/remove on leave
    - [ ] Provide getters (getPlayerData)

---

## ⏱️ Cooldown System

- [ ] Create CooldownManager
    - [ ] Store cooldowns per player
    - [ ] Check if on cooldown
    - [ ] Start cooldown
    - [ ] Get remaining time

- [ ] Support multiple cooldown types
    - [ ] Ability cooldown
    - [ ] Weapon cooldown

---

## ⚡ Ability System

- [ ] Create Ability interface
- [ ] Implement abilities:
    - [ ] PhantomModeAbility
    - [ ] BlinkAbility
    - [ ] ScanAbility

- [ ] Create AbilityManager
    - [ ] Register abilities
    - [ ] Activate ability
    - [ ] Handle cooldown integration

---

## 🔫 Weapon System

- [ ] Create Weapon interface
- [ ] Implement weapons:
    - [ ] Rifle
    - [ ] Shotgun
    - [ ] Sniper

- [ ] Create WeaponManager
    - [ ] Handle shooting
    - [ ] Handle hit detection
    - [ ] Apply damage

---

## 🩸 Combat System

- [ ] Create DamageManager
    - [ ] Apply damage
    - [ ] Handle death
    - [ ] Track killer

- [ ] Add hit validation
    - [ ] Range check
    - [ ] Friendly fire rules

---

## 👻 Phantom Mode System

- [ ] Track phantom state per player
- [ ] Apply effects:
    - [ ] Speed boost
    - [ ] Invulnerability
- [ ] Disable shooting while active
- [ ] Auto-disable after duration

---

## 🎮 Game System

- [ ] Create GameState enum (LOBBY, RUNNING, END)
- [ ] Create GameManager
    - [ ] Start game
    - [ ] End game
    - [ ] Track players
    - [ ] Handle respawns

---

## 🧮 Score System

- [ ] Track kills
- [ ] Track deaths
- [ ] Add score calculation
- [ ] Provide leaderboard data

---

## 🔄 Event Integration

- [ ] Connect PlayerJoinEvent → PlayerDataManager
- [ ] Connect PlayerQuitEvent → cleanup
- [ ] Connect damage events → DamageManager

---

## 🧪 Testing

- [ ] Test each system independently
- [ ] Test ability + cooldown interaction
- [ ] Test multiplayer combat
- [ ] Test edge cases (disconnects, spam)

---
