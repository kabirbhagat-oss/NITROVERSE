# 🏎️ NITROVERSE - Multiplayer Racing Game

A high-performance **3D peer-to-peer multiplayer racing game** built with **Unity** and **Photon PUN 2** for **iOS & Android**.

## 🎮 Features

- **2-4 Player Peer-to-Peer Racing** - Real-time multiplayer synchronization
- **3D Realistic Physics** - Car dynamics, collision detection, drift mechanics
- **Mobile Optimized** - Touch controls for iOS and Android
- **Dynamic Race Tracking** - Lap counting, checkpoints, leaderboards
- **Customizable Cars** - Different vehicle classes and skins
- **Multiple Tracks** - Diverse racing environments
- **Real-time Networking** - Low-latency P2P communication via Photon
- **Cross-Platform** - Play iOS vs Android seamlessly

## 🛠️ Tech Stack

- **Engine:** Unity 2022 LTS or higher
- **Networking:** Photon PUN 2
- **Platform:** iOS & Android
- **Physics:** Unity PhysX
- **UI Framework:** Unity UI (uGUI)

## 📁 Project Structure

```
Assets/
├── Scripts/
│   ├── Networking/          # Photon integration & P2P logic
│   ├── Racing/              # Car physics & race mechanics
│   ├── UI/                  # UI managers & menus
│   ├── Input/               # Mobile input handlers
│   └── Managers/            # Game state & managers
├── Scenes/
│   ├── Lobby.unity
│   ├── Track_01.unity
│   └── Track_02.unity
├── Prefabs/
│   ├── Car.prefab
│   ├── Player.prefab
│   └── UI/
├── Resources/
│   └── Photon/              # Photon configuration
└── Materials & Textures/

ProjectSettings/
.gitignore
DEVELOPMENT.md              # Setup & development guide
```

## 🚀 Quick Start

### Prerequisites
- Unity 2022 LTS or higher
- Photon PUN 2 asset (from Asset Store)
- iOS/Android build support

### Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/kabirbhagat-oss/NITROVERSE.git
   cd NITROVERSE
   ```

2. **Open in Unity**
   - Unity version: 2022 LTS or higher
   - Platform: iOS/Android

3. **Import Photon PUN 2**
   - Asset Store > Search "Photon PUN 2"
   - Import to project
   - Configure AppId in `Resources/Photon/PhotonServerSettings`

4. **Build & Deploy**
   - iOS: File > Build Settings > iOS > Build
   - Android: File > Build Settings > Android > Build

See **DEVELOPMENT.md** for detailed setup instructions.

## 🎯 Game Flow

1. **Lobby System** - Join/create multiplayer sessions
2. **Track Selection** - Choose racing environment
3. **Car Customization** - Select vehicle and setup
4. **Race Loading** - Synchronized player spawning
5. **Live Racing** - Real-time multiplayer competition
6. **Results Screen** - Leaderboard & statistics

## 🔧 Core Systems

### Networking (Photon PUN 2)
- Room management for 2-4 players
- OnPhotonSerializeView for position sync
- Remote Procedure Calls (RPCs) for events
- Network instantiation of cars

### Racing Mechanics
- Vehicle physics with acceleration, braking, steering
- Drift mechanics with speed boost
- Collision detection
- Lap timing and checkpoint tracking
- AI opponent support (optional)

### Input System
- Touch-based steering (tilt or tap-to-steer)
- Accelerate/Brake buttons
- Power-up activation
- Pause/menu controls

## 📊 Network Sync

**Synchronized Properties:**
- Player position & rotation
- Car velocity & acceleration
- Input state
- Lap count & race position
- Collision events

**Update Rate:** 20 updates/second (configurable)

## 🎨 Customization

Edit game settings in:
- `Scripts/Managers/GameConfig.cs` - Game parameters
- `Resources/Photon/PhotonServerSettings` - Photon configuration
- Scene settings for track-specific adjustments

## 📱 Mobile Optimization

- Optimized draw calls
- LOD (Level of Detail) systems
- Memory pooling for objects
- Target: 60 FPS on mid-range devices

## 🤝 Contributing

1. Create a feature branch (`git checkout -b feature/racing-feature`)
2. Commit changes (`git commit -m 'Add racing feature'`)
3. Push to branch (`git push origin feature/racing-feature`)
4. Open a Pull Request

## 📝 License

MIT License - see LICENSE file for details

## 🐛 Known Issues & Roadmap

### Current Version (v0.1)
- [x] Basic car physics
- [x] P2P networking
- [x] Lap tracking
- [ ] Power-ups system
- [ ] AI opponents
- [ ] Cosmetic customization
- [ ] Seasonal events

### Roadmap
- Better network interpolation
- Advanced car physics
- More tracks
- Mobile controller support
- Clan/tournament system

## 📞 Support

For issues and feature requests, please open an issue on GitHub.

---

**Made with ❤️ for racing enthusiasts** 🏁
