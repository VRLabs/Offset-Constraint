<div align="center">

# Offset Constraint

[![Generic badge](https://img.shields.io/github/downloads/VRLabs/Offset-Constraint/total?label=Downloads)](https://github.com/VRLabs/Offset-Constraint/releases/latest)
[![Generic badge](https://img.shields.io/badge/License-MIT-informational.svg)](https://github.com/VRLabs/Offset-Constraint/blob/main/LICENSE)
[![Generic badge](https://img.shields.io/badge/Quest-Compatible-green?logo=Meta)](https://img.shields.io/badge/Quest-Compatible-green?logo=Meta)
[![Generic badge](https://img.shields.io/badge/Unity-2022.3.22f1-lightblue?logo=Unity)](https://unity.com/releases/editor/whats-new/2022.3.22)
[![Generic badge](https://img.shields.io/badge/SDK-AvatarSDK3-lightblue.svg)](https://vrchat.com/home/download)

[![Generic badge](https://img.shields.io/discord/706913824607043605?color=%237289da&label=DISCORD&logo=Discord&style=for-the-badge)](https://discord.vrlabs.dev/)
[![Generic badge](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fshieldsio-patreon.vercel.app%2Fapi%3Fusername%3Dvrlabs%26type%3Dpatrons&style=for-the-badge)](https://patreon.vrlabs.dev/)

A constraint system to preserve offsets

![OffsetConstraint](https://github.com/VRLabs/Offset-Constraint/assets/76777936/f38a68f8-c502-4008-a6ba-7820c08d6232)

### ⬇️ [Download Latest Version](https://github.com/VRLabs/Offset-Constraint/releases/latest)

### 📦 [Add to VRChat Creator Companion](https://vrlabs.dev/packages?package=dev.vrlabs.offset-constraint)

</div>

---

## How it works

* Uses native VRCConstraint components to preserve offset transforms via the "Rebake Offsets When Unfrozen" setting.
* Offsets are reset by swapping to a secondary source that mirrors the original but maintains zero offsets, preventing unintended rebakes.

## Install guide

https://github.com/VRLabs/Offset-Constraint/assets/76777936/f20790ad-0a5e-49ee-aaac-3b2e380f5f93

* Merge the Animator Controller ``Offset Constraint FX`` to your own FX Controller, using the [Avatars 3.0 Manager](https://github.com/VRLabs/Avatars-3.0-Manager) tool.
* Drag & drop the ``Offset Constraint`` prefab into the base of your Hierarchy.
* Right click and unpack the prefab, then drag & drop it onto your avatar.
* Expand the prefab hierarchy and find ``Offset Target``
* Move ``Offset Target`` outside of ``Offset Constraint`` and place it anywhere in your avatars hierarchy as needed.

> [!NOTE]  
> When building for Quest, you will have to remove unsupported components and shaders

## How to use

* Place the objects you want to use inside ``Offset Constraint``.
  * Alternatively you can constrain the objects to ``Offset Constraint``.

There are two bools in your FX Controller:

* ``OffsetConstraint/Control``:
  * True: Places ``Offset Constraint`` in world space and allows the user to generate an offset.
  * False: Constrains the ``Offset Constraint`` to the ``Offset Target`` with the generated offset.
* ``OffsetConstraint/Reset`` moves ``Offset Constraint`` to the ``Offset Target``.

## Performance stats

```c++
Constraints:        1
FX Animator Layers: 1
```

## Hierarchy layout

```html
Offset Constraint
|-Cube
|-Offset Target
```

## Contributors

* [lin](https://github.com/oofdesu)

## License

Offset Constraint is available as-is under MIT. For more information see [LICENSE](https://github.com/VRLabs/Offset-Constraint/blob/main/LICENSE).

​

<div align="center">

[<img src="https://github.com/VRLabs/Resources/raw/main/Icons/VRLabs.png" width="50" height="50">](https://vrlabs.dev "VRLabs")
<img src="https://github.com/VRLabs/Resources/raw/main/Icons/Empty.png" width="10">
[<img src="https://github.com/VRLabs/Resources/raw/main/Icons/Discord.png" width="50" height="50">](https://discord.vrlabs.dev/ "VRLabs")
<img src="https://github.com/VRLabs/Resources/raw/main/Icons/Empty.png" width="10">
[<img src="https://github.com/VRLabs/Resources/raw/main/Icons/Patreon.png" width="50" height="50">](https://patreon.vrlabs.dev/ "VRLabs")
<img src="https://github.com/VRLabs/Resources/raw/main/Icons/Empty.png" width="10">
[<img src="https://github.com/VRLabs/Resources/raw/main/Icons/Twitter.png" width="50" height="50">](https://twitter.com/vrlabsdev "VRLabs")

</div>
