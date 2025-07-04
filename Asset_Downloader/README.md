<div align="center">
  <img src="https://github.com/Toxocious/Absolute/raw/master/app/images/Assets/banner.png" title="Pokemon Absolute Logo" alt="Pokemon Absolute Logo" />
  <h1 align="center">Pok&eacute;mon Absolute &mdash; Asset Downloader</h1>

  **Absolute's Asset Downloader** is an TypeScript tool used to fetch and download assets from [Pokemon Showdown](https://play.pokemonshowdown.com/).

  <img alt="Github Issues" src="https://img.shields.io/github/issues/PokemonAbsolute/Absolute-Tools?style=for-the-badge&logo=appveyor" />
  <img alt="Github Forks" src="https://img.shields.io/github/forks/PokemonAbsolute/Absolute-Tools?style=for-the-badge&logo=appveyor" />
  <img alt="Github Stars" src="https://img.shields.io/github/stars/PokemonAbsolute/Absolute-Tools?style=for-the-badge&logo=appveyor" />
  <br />

  <img alt="GitHub contributors" src="https://img.shields.io/github/contributors/PokemonAbsolute/Absolute-Tools?style=for-the-badge">
  <a href="https://visitorbadge.io/status?path=https%3A%2F%2Fgithub.com%2FToxocious%2FAbsolute-Chat">
    <img src="https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2FToxocious%2FAbsolute-Chat&label=VIEWS&countColor=%234a618f" />
  </a>
  <br />

  <img alt="License" src="https://img.shields.io/github/license/PokemonAbsolute/Absolute-Tools?style=for-the-badge&logo=appveyor" />

  Come join our comfy community over on Discord!

  <a href="https://discord.gg/SHnvbsS" target="_blank">
    <img src="https://discord.com/api/guilds/269182206621122560/widget.png?style=banner2" alt="Discord Invite Banner" />
  </a>
</div>



# Table of Contents
- [Table of Contents](#table-of-contents)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Output Structure](#output-structure)
- [License](#license)
- [Legal Notice](#legal-notice)



# Features
- Multi-threaded downloads for optimal performance
- Automatic directory creation and organization
- Configurable asset categories
- CPU-aware thread management



# Requirements
- Node.js (v14 or higher recommended)
- NPM or Yarn package manager



# Installation
1. Navigate to the Tools/Asset_Downloader directory
2. Install dependencies:

```bash
npm install
```



# Usage
Run the tool with:

```bash
npm start
```

or

```typescript
npx ts-node Asset_Downloader.ts
```



# Configuration
The tool downloads sprites from configurable source directories. Edit the `sourceDirectories` array in Asset_Downloader.ts to customize which sprite collections are downloaded.

```typescript
const sourceDirectories = [
    {
        url: 'https://play.pokemonshowdown.com/sprites/gen5/',
        outputDir: './Sprites/Normal',
    },
    {
        url: 'https://play.pokemonshowdown.com/sprites/types/',
        outputDir: './Sprites/Types',
    },
];
```



# Output Structure
Downloaded assets are organized into the following directory structure:

```
./Audio/
  ├── Cries/        - All cries for Pokemon in .wav format
./Sprites/
  ├── Normal/       - Regular Pokémon sprites
  ├── Normal-Backs/ - Back-facing regular sprites
  ├── Shiny/        - Shiny Pokémon sprites
  ├── Shiny-Backs/  - Back-facing shiny sprites
  ├── Items/        - Item icons
  ├── Categories/   - Move category icons
  └── Types/        - Type icons
```


# License
This tool is part of the Absolute project and is subject to the license terms specified in the main repository's [LICENSE](https://github.com/PokemonAbsolute/Absolute/blob/master/LICENSE).



# Legal Notice
I do **not** claim to own any assets that are downloaded via use of this tool.

All Pokémon sprites and assets are owned by The Pokémon Company International and Nintendo.

Please respect copyright laws when using downloaded assets.
