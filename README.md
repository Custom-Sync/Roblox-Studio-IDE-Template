# Roblox Studio IDE Template

A modern development template for creating Roblox games using external IDEs with [Rojo](https://rojo.space/) synchronization.

## 🚀 Summit Studios Challenge

This project is part of the **Summit Studios Windsurf Challenge**! Learn more and participate at:
**[Summit Studios Windsurf Challenge](https://www.summitstudios.io/challenge-page/windsurf?programId=c6b96e0e-033e-42a1-8e64-225b05e898dc)**

## 📋 Overview

This template provides a structured foundation for developing Roblox games outside of Roblox Studio, enabling developers to use modern IDEs with better tooling, version control, and collaborative features.

## 🛠️ Tools & Configuration

### Development Tools (managed by Aftman)
- **[Rojo 7.4.0](https://rojo.space/)** - File synchronization between IDE and Roblox Studio
- **[Selene 0.25.0](https://kampfkarren.github.io/selene/)** - Lua linter for code quality
- **[StyLua 0.18.2](https://github.com/JohnnyMorganz/StyLua)** - Lua code formatter

### Configuration Files
- `default.project.json` - Rojo project configuration mapping local folders to Roblox services
- `aftman.toml` - Tool version management
- `selene.toml` - Linting rules and code quality standards
- `stylua.toml` - Code formatting configuration
- `globalTypes.d.luau` - TypeScript-style type definitions for Luau

## 📁 Project Structure

```
src/
├── Lighting/                    # Lighting configuration and scripts
├── Players/                     # Player-related functionality
├── ReplicatedFirst/            # Scripts that run before character spawning
├── ReplicatedStorage/          # Shared resources between server and client
├── ServerScriptService/        # Server-side scripts and logic
├── ServerStorage/              # Server-only resources and data  
├── SoundService/               # Audio management and configuration
├── StarterGui/                 # UI elements copied to players
├── StarterPack/                # Tools given to players on spawn
├── StarterPlayerScripts/       # Client-side scripts for each player
├── StarterCharacterScripts/    # Scripts attached to player characters
├── Teams/                      # Team configuration and management
└── Workspace/                  # 3D world objects and scripts
```

## 🚀 Getting Started

### Prerequisites
- [Roblox Studio](https://create.roblox.com/docs/studio/setting-up-roblox-studio)
- [Aftman](https://github.com/LPGhatguy/aftman) for tool management

### Setup Instructions

1. **Install Aftman** (if not already installed):
   ```bash
   # Install Aftman following their official documentation
   ```

2. **Install project tools**:
   ```bash
   aftman install
   ```

3. **Start Rojo server**:
   ```bash
   rojo serve
   ```

4. **Connect to Roblox Studio**:
   - Open Roblox Studio
   - Install the Rojo plugin if you haven't already
   - Click the Rojo plugin and connect to `localhost:34872`

## 💻 Development Workflow

1. **Write Code**: Develop in your preferred IDE using the organized folder structure
2. **Live Sync**: Rojo automatically syncs changes to Roblox Studio in real-time
3. **Code Quality**: Use Selene for linting and catch potential issues
4. **Formatting**: Run StyLua to maintain consistent code style
5. **Version Control**: Leverage Git for proper version management

## 📝 Code Quality

### Linting with Selene
```bash
selene src/
```

### Formatting with StyLua
```bash
stylua src/
```

## 🎮 Features

- **Modern IDE Support**: Use VS Code, IntelliJ, or any preferred editor
- **Real-time Sync**: Changes appear instantly in Roblox Studio
- **Code Quality Tools**: Built-in linting and formatting
- **Type Safety**: Luau type definitions for better development experience
- **Version Control Ready**: Git-friendly structure and .gitignore
- **Team Collaboration**: Consistent tooling and code standards

## 🤝 Contributing

This project follows the standards and practices established for the Summit Studios Windsurf Challenge. When contributing:

1. Follow the established code style (enforced by StyLua)
2. Ensure code passes linting (Selene)
3. Test changes in Roblox Studio
4. Submit pull requests with clear descriptions

## 📄 License

See [LICENSE](LICENSE) file for details.

## 🔗 Resources

- [Rojo Documentation](https://rojo.space/docs/)
- [Luau Language Guide](https://luau-lang.org/)
- [Roblox Creator Documentation](https://create.roblox.com/docs/)
- [Summit Studios](https://www.summitstudios.io/)

---

**Happy coding and good luck with the Summit Studios Windsurf Challenge! 🌊**
