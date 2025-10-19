# The Nonexistence of You and Me — Asset Research

This repository documents the internal Unity asset structure of the visual novel *The Nonexistence of You and Me*, analyzed for educational and archival purposes.

The goal of this project is to understand and document how various Unity asset types (such as `AudioClip`, `Texture2D`, `Shader`, and `TextAsset`) are organized and used in a commercial VN‐style build, without redistributing or modifying the original copyrighted content.

> ⚠️ **Disclaimer:**  
> This project is purely for **technical analysis, learning, and preservation**.  
> No playable or redistributable game assets (full models, textures, music, or full scripts) are shared here. All content here is limited to metadata, file paths, format specifications, and small excerpts for commentary.

---

## Repository Structure

- `AudioClip/` : Metadata relating to in‐game audio (voice lines, sound effects, background music).  
- `AudioMixerController/`, `AudioMixerEffectController/`, `AudioMixerGroupController/`, `AudioMixerSnapshotController/` : Audio mixing, routing and snapshot configurations used by Unity’s sound system.  
- `EditorSettings/` : Editor‐specific configuration data (may contain leftover dev settings).  
- `Font/` : References to font assets used in the UI and text rendering.  
- `LightmapParameters/` : Unity lightmap configuration metadata (likely minimal use in VN scenes).  
- `Mesh/` : Mesh descriptors for any 3D/2.5D uses if present.  
- `PrefabHierarchyObject/` : Prefab definitions and scene‐object hierarchies for UI and scene layouts.  
- `Shader/` : Shader definitions for UI/material effects, transitions, lighting.  
- `Sprite/` : 2D sprite metadata used for UI, characters, backgrounds.  
- `Texture2D/` : Texture metadata (diffuse maps, UI assets, background images).  
- `TextAsset/` : Textual data including localization, script files, and internal/test files.  
- `VideoClip/` : Metadata for video assets (intro/cutscenes/outro segments).  

---

## Analysis Goals

- Reverse‐engineer how Unity organizes narrative and multimedia content within `.bytes`, `.asset`, `.bundle`, `.resS` containers.  
- Study file naming conventions and how different asset types link to each other.  
- Document and highlight unused or test content discovered in the build.  
- Share patterns and insights useful for educational reference and archival documentation.

---

## Tools & Environment

Analysis was performed using the following tools:

- UABEAvalonia

## License

Licensed under the MIT License.  
All brand names, trademarks, and copyrighted materials belong to their respective owners.
