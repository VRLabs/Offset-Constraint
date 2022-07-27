# Offset Constraint
  
[![Generic badge](https://img.shields.io/badge/Unity-2019.4.31f1-informational.svg)](https://unity3d.com/unity/whats-new/2019.4.31)
[![Generic badge](https://img.shields.io/badge/SDK-AvatarSDK3-informational.svg)](https://vrchat.com/home/download)
[![Generic badge](https://img.shields.io/badge/License-MIT-informational.svg)](https://github.com/VRLabs/Offset-Constraint/blob/main/LICENSE)
[![Generic badge](https://img.shields.io/github/downloads/VRLabs/Offset-Constraint/total?label=Downloads)](https://github.com/VRLabs/Offset-Constraint/releases/latest)

A hierarchy of animated constraints that display how to move an object in world space while preserving previously generated offsets.

## How it works

Constraints reference each other as sources and swap their enabled state to preserved offset transforms.

## Install guide

Merge the FX controller to your own FX controller, using the [Avatars 3.0 Manager](https://github.com/VRLabs/Avatars-3.0-Manager) tool.

"Offset Constraint.prefab" should go to the base of your Unity scene, which will give it base Unity scaling.

Unpack the prefab by right-clicking it and move the prefab to base of your avatar.

Expand the prefab, and locate "Offset Target". Move this object out of the prefab to anywhere else on your avatar.

## How to use

"OffsetConstraint.Control" will allow the "Container" transform to move when the value is False. The Container will be left in the world when OffsetConstraint.Control is True.

"OffsetConstraint.Reset" will override OffsetConstraint.Control and reset the Container to the Offset Target.

The default value is False. 

## Downloads

You can grab the latest version of the Offset Constraint in [Releases](https://github.com/VRLabs/Offset-Constraint/releases/latest).

## License

Offset Constraint is available as-is under MIT. For more information see [LICENSE](https://github.com/VRLabs/Offset-Constraint/blob/main/LICENSE).

## Contact us

If you need help, our support channel is on [Discord](https://discord.vrlabs.dev).
