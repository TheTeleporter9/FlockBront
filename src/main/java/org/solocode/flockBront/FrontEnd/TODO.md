# 🎮 Phantom Trigger Plugin - Development TODO

---

## 🧠 Backend (Systems)

### Core Systems
- [ ] Create AbilityManager
- [ ] Create WeaponManager
- [ ] Create Cooldown system
- [ ] Create PlayerData system (store player state)

### Combat
- [ ] Implement shooting system (projectiles / raycast)
- [ ] Add damage handling
- [ ] Add hit detection

### Phantom Mechanic
- [ ] Implement Phantom Mode toggle
- [ ] Add duration + cooldown
- [ ] Prevent shooting while in Phantom Mode
- [ ] Add movement modifier

### Game Logic
- [ ] Create GameManager (game states: LOBBY, RUNNING, END)
- [ ] Handle player join/leave
- [ ] Implement respawn system
- [ ] Add scoring system

---

## 🎨 Frontend (Player Experience)

### Commands
- [ ] /pt join
- [ ] /pt leave
- [ ] /pt start
- [ ] /pt kit

### GUI
- [ ] Create Weapon Select Menu
- [ ] Create Ability Select Menu
- [ ] Handle inventory clicks
- [ ] Highlight selected items

### Visual Feedback
- [ ] Add particles for shooting
- [ ] Add Phantom Mode particles
- [ ] Add hit effects

### Sound
- [ ] Add shooting sound
- [ ] Add ability activation sound
- [ ] Add hitmarker sound

### Messages
- [ ] Send action bar updates (cooldowns, ammo)
- [ ] Send join/leave messages
- [ ] Send ability feedback ("On cooldown!")

### HUD
- [ ] Create scoreboard system
- [ ] Display kills / deaths
- [ ] Display ability cooldown

---

## 🔗 Integration (IMPORTANT)

- [ ] Connect GUI → AbilityManager
- [ ] Connect commands → GameManager
- [ ] Connect input events → WeaponManager
- [ ] Sync PlayerData with frontend display

---

## 🧪 Testing

- [ ] Test abilities in isolation
- [ ] Test multiplayer interactions
- [ ] Test cooldown edge cases
- [ ] Test GUI clicks spam

---

## 🚀 Polish

- [ ] Add titles (game start/end)
- [ ] Add animations (particles, sounds)
- [ ] Balance weapons
- [ ] Optimize performance

---
