---
id: "Tweening.MotionConfig"
title: "Interface: MotionConfig<T>"
sidebar_label: "MotionConfig"
custom_edit_url: null
---

[Tweening](../namespaces/Tweening.md).MotionConfig

Interface for configuring motion animations in a Tween.
You can specify easing, callback functions, and progress tracking functions.

## Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `T` | `any` | The type of the target object being tweened. |

## Properties

### easing

• `Optional` **easing**: [`Easing`](../namespaces/Tweening.md#easing)

The easing function to control the animation's progression.

#### Defined in

[src/tweening/Actions.ts:24](https://github.com/agargaro/three.ez/blob/0027204/src/tweening/Actions.ts#L24)

___

### onComplete

• `Optional` **onComplete**: (`target`: `T`) => `void`

#### Type declaration

▸ (`target`): `void`

A callback function to execute when the animation completes.

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `T` | The target object that was tweened. |

##### Returns

`void`

#### Defined in

[src/tweening/Actions.ts:29](https://github.com/agargaro/three.ez/blob/0027204/src/tweening/Actions.ts#L29)

___

### onProgress

• `Optional` **onProgress**: (`target`: `T`, `key`: `string`, `start`: `AllowedTypes`, `end`: `AllowedTypes`, `alpha`: `number`) => `boolean` \| `void`

#### Type declaration

▸ (`target`, `key`, `start`, `end`, `alpha`): `boolean` \| `void`

A callback function to be executed before each property is updated.

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `T` | The target object that is being tweened. |
| `key` | `string` | The key or property being animated. |
| `start` | `AllowedTypes` | The initial value of the animated property. |
| `end` | `AllowedTypes` | The final value of the animated property. |
| `alpha` | `number` | The current animation progress as a normalized value (0 to 1). |

##### Returns

`boolean` \| `void`

If `false`, will not assign a new value to the property.

#### Defined in

[src/tweening/Actions.ts:49](https://github.com/agargaro/three.ez/blob/0027204/src/tweening/Actions.ts#L49)

___

### onStart

• `Optional` **onStart**: (`target`: `T`) => `void`

#### Type declaration

▸ (`target`): `void`

A callback function to execute when the animation starts.

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `T` | The target object that is being tweened. |

##### Returns

`void`

#### Defined in

[src/tweening/Actions.ts:34](https://github.com/agargaro/three.ez/blob/0027204/src/tweening/Actions.ts#L34)

___

### onUpdate

• `Optional` **onUpdate**: (`target`: `T`) => `void`

#### Type declaration

▸ (`target`): `void`

A callback function to be executed after each property has been updated.

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `target` | `T` | The target object that is being tweened. |

##### Returns

`void`

#### Defined in

[src/tweening/Actions.ts:39](https://github.com/agargaro/three.ez/blob/0027204/src/tweening/Actions.ts#L39)
