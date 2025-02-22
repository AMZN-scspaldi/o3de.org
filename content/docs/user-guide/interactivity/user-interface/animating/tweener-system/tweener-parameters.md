---
description: ' Learn how to modify Lua script parameters in the Scripted Entity Tweener
  system for Open 3D Engine. '
title: Tweener Parameters
---

Scripted Entity Tweener parameters provide flexibility and allow you to customize your tweener animations. Use the parameters with a [timeline](tweener-timeline/) for a variety of possibilities.

Use the following tweener parameters to customize your animation.

**duration**
Specifies the time in seconds for the animation to go from the start value to its final value.

**\["x"\] and \["y"\]**
Shortcuts for the `x` and `y` values of a `UiTransform2dComponent`, which is automatically attached to every UI entity.

**timeIntoTween**
Specifies a tween to begin at a specified point (in seconds). For example, if the `duration` is set to `6`, and `timeIntoTween` is set to `3`, then the tween begins immediately at its halfway point and finishes in three more seconds.

**easeMethod **
Specifies the [easing type](tweener-understanding-types/) to apply to the tween.
+ `ScriptedEntityTweenerEasingMethod_Linear`
+ `ScriptedEntityTweenerEasingMethod_Quad`
+ `ScriptedEntityTweenerEasingMethod_Cubic`
+ `ScriptedEntityTweenerEasingMethod_Quart`
+ `ScriptedEntityTweenerEasingMethod_Quint`
+ `ScriptedEntityTweenerEasingMethod_Sine`
+ `ScriptedEntityTweenerEasingMethod_Expo`
+ `ScriptedEntityTweenerEasingMethod_Circ`
+ `ScriptedEntityTweenerEasingMethod_Elastic`
+ `ScriptedEntityTweenerEasingMethod_Back`
+ `ScriptedEntityTweenerEasingMethod_Bounce`

**easeType**
Modifies `easeMethod`.
+ `ScriptedEntityTweenerEasingType_In`
+ `ScriptedEntityTweenerEasingType_Out`
+ `ScriptedEntityTweenerEasingType_InOut`

**delay**
Specifies an amount of time in seconds to delay the start of the animation.

**timesToPlay**
Number of times to play the animation. Specify `-1` to play the animation indefinitely.

**isFrom**
If `false`, the animation starts at the value specified in the component and ends at the value specified in the script.
If `true`, the animation starts at the value specified in the script and ends at the value specified in the component.

**isPlayingBackward**
If `true`, the animation plays backwards. To play an animation backward, you must specify a value for `timeIntoTween`. If a value is not specified for `timeIntoTween`, this parameter is ignored.

**uuid**
ID generated by the Scripted Entity Tweener system and used for debugging purposes. You do not need to modify or specify a value.

**onComplete, onUpdate, and onLoop**
Use these parameters to specify a callback function when the animation completes, updates, or loops. `onUpdate` also passes back the animation's current completion state percentage and the current value of the animated parameter.
