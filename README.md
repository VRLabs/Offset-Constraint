<div align="center">

# Offset Constraint

[![Generic badge](https://img.shields.io/github/downloads/VRLabs/Offset-Constraint/total?label=Downloads)](https://github.com/VRLabs/Offset-Constraint/releases/latest)
[![Generic badge](https://img.shields.io/badge/License-MIT-informational.svg)](https://github.com/VRLabs/Offset-Constraint/blob/main/LICENSE)
[![Generic badge](https://img.shields.io/badge/Unity-2019.4.31f1-lightblue.svg)](https://unity3d.com/unity/whats-new/2019.4.31)
[![Generic badge](https://img.shields.io/badge/SDK-AvatarSDK3-lightblue.svg)](https://vrchat.com/home/download)

[![Generic badge](https://img.shields.io/discord/706913824607043605?color=%237289da&label=DISCORD&logo=Discord&style=for-the-badge)](https://discord.vrlabs.dev/)
[![Generic badge](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fshieldsio-patreon.vercel.app%2Fapi%3Fusername%3Dvrlabs%26type%3Dpatrons&style=for-the-badge)](https://patreon.vrlabs.dev/)

A constraint system to preserve offsets

![OffsetConstraint](https://github.com/VRLabs/Offset-Constraint/assets/76777936/80749a88-a705-4243-8552-590cd70d327f)


### ⬇️ [Download latest Unitypackage](https://github.com/VRLabs/Offset-Constraint/releases/latest)

<!-- 
### 📦 [Add to VRChat Creator Companion]() -->

</div>

---

## How it works

* Constraints reference each other as sources and swap their enabled state to preserve offset transforms.

## Install guide

https://github.com/VRLabs/Offset-Constraint/assets/76777936/f20790ad-0a5e-49ee-aaac-3b2e380f5f93

* Merge the Animator Controller ``Offset Constraint FX`` to your own FX Controller, using the [Avatars 3.0 Manager](https://github.com/VRLabs/Avatars-3.0-Manager) tool.
* Drag & drop the ``Offset Constraint`` prefab into the base of your Hierarchy.
* Right click and unpack the prefab, then drag & drop it onto your avatar.
* Expand the prefab hierarchy and find ``Offset Target``
* Move ``Offset Target`` outside of ``Offset Constraint`` and place it anywhere in your avatars hierarchy as needed.

## How to use

* Place the objects you want to to use inside ``Offset Constraint`` -> ``Container``.
  * Alternatively you can constrain the objects to ``Container``.

There are two bools in your FX Controller:

* ``OffsetConstraint/Control``:
  * True: Places the ``Container`` in world space and allows the user to set the specified offset.
  * False: Constraints the ``Container`` to the ``Offset Target`` with the specified offset.
* ``OffsetConstraint/Reset`` moves the ``Container`` to the ``Offset Target``.

## Performance stats

```c++
Constraints:        2
FX Animator Layers: 1
```

## Hierarchy layout

```html
Offset Constraint
|-Container
|  |-Cube
|-Root
|  |-End
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

---
