# Contributing to Lucky Block Mod

Thank you for your interest in contributing to the Lucky Block Mod for Minecraft Bedrock!

## Code of Conduct

Please be respectful and inclusive when interacting with other contributors.

## How to Contribute

### Reporting Bugs

1. Check if the bug has already been reported
2. Create a new issue with:
   - Clear title
   - Detailed description
   - Steps to reproduce
   - Expected vs actual behavior
   - Device and Minecraft version
   - Screenshots/videos if helpful

### Suggesting Features

1. Check if the feature has already been suggested
2. Create a new issue with:
   - Clear title
   - Feature description
   - Why this feature would be useful
   - How it might work

### Submitting Pull Requests

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/my-feature`
3. Make your changes
4. Test thoroughly in Minecraft
5. Commit with clear messages: `git commit -m "Add feature X"`
6. Push to your fork: `git push origin feature/my-feature`
7. Open a pull request with:
   - Clear title
   - Description of changes
   - Any related issues

## Development Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/kumarikhushbo175-eng/lucky-blck.git
   cd lucky-blck
   ```

2. Copy packs to Minecraft directory:
   - Windows: `%appdata%/Microsoft/Windows/AppsLocal/Microsoft.MinecraftUWP_8wekyb3d8bbwe/Local State/games/com.mojang/`
   - Or use symbolic links

3. Test in Minecraft

## File Structure

```
lucky-blck/
├── behavior_pack/          # Game logic
│   ├── manifest.json       # Pack metadata
│   ├── blocks/             # Block definitions
│   ├── entities/           # Entity definitions
│   ├── loot_tables/        # Item rewards
│   └── functions/          # Events and commands
├── resource_pack/          # Visuals and sounds
│   ├── manifest.json       # Pack metadata
│   ├── textures/           # Block textures
│   └── sounds.json         # Sound definitions
├── docs/                   # Documentation
│   ├── INSTALLATION.md     # Setup guide
│   └── CUSTOMIZATION.md    # Modification guide
├── README.md               # Project overview
├── CHANGELOG.md            # Version history
└── CONTRIBUTING.md         # This file
```

## Coding Standards

- Use consistent JSON formatting
- Add comments for complex sections
- Test all changes in-game
- Keep file sizes reasonable
- Follow Minecraft Bedrock conventions

## Testing Checklist

Before submitting a PR:
- [ ] Tested in creative mode
- [ ] Tested in survival mode
- [ ] Tested with multiplayer
- [ ] No console errors
- [ ] Changes don't break existing features
- [ ] Documentation is updated

## Questions?

- Open an issue for discussion
- Contact the maintainer
- Check existing documentation

## License

By contributing, you agree that your contributions will be licensed under the MIT License.

Thank you for making Lucky Block Mod better! 🎮✨
