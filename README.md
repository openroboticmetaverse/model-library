<p align="center">
  <a href="https://www.openroboticmetaverse.org">
    <img alt="orom" src="https://raw.githubusercontent.com/openroboverse/knowledge-base/main/docs/assets/icon.png" width="100" />
  </a>
</p>
<h1 align="center">
  🤖 open robotic metaverse mvp - model library 🌐
</h1>

## Overview 🔍

This repo temporarily hosts robot and objects models for visualisation in the orom mvp webapp.

## Folder Structure 📂

- `objects/` directory contains various object models.
  - `gltf/` subdirectory contains GLTF models.
- `robots/` directory contains robot models.
  - `gltf/` subdirectory contains GLTF models.
  - `mujoco/` subdirectory contains MJCF models.
  - `urdf/` subdirectory contains URDF models.
- `ref_library.json` configuration file contains metadata about the models.

## Adding Models 🛠️

To add a new model to the repository, follow these steps:

1. **Add the model files**:

   - Place the model files in the appropriate subdirectory (e.g., `robots/urdf`, `objects/gltf`, ...).

2. **Update the config file `ref_library.json`**:
   - Add an entry for the new model in the `robots` or `objects` array.
   - Include the following fields:
     - `name`: The name of the model.
     - `file`: The absolute path to the model file starting from the root of the repository. e.g. "/robots/mujoco/franka_emika_panda/panda.xml"
     - `file_type`: The type of the model file (e.g., `gltf`, `mjcf`, `urdf`).
     - `description`: A brief description of the model.
     - `created_at`: The creation date of the model entry.
     - `updated_at`: The last update date of the model entry.

## Attribution ©️

- The robot models are subject to the copyright of their respective owners.

- The Franka, Sawyer and Niryo URDF files are adapted from https://github.com/ndahn/Rocksi

- MuJoCo models are form the [google-deepmind/mujoco_menagerie](https://github.com/google-deepmind/mujoco_menagerie)
- Motorcortex Robot models are used with permission from [Vectioneer](https://vectioneer.com/)
