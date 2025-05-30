[@scrolia/vanilla](../README.md) / createScrollbar

# Function: createScrollbar()

```ts
function createScrollbar(options?): CreateScrollbar;
```

Defined in: [packages/vanilla/src/base/index.ts:78](https://github.com/alpheusday/scrolia/blob/a1d15b8008e894d5dd6b0e61a1c2164d92ca7b98/packages/vanilla/src/base/index.ts#L78)

Function to create the scrollbar.

### Example

```ts
import type { CreateScrollbar } from "@scrolia/vanilla";

import { createScrollbar } from "@scrolia/vanilla";

const el: HTMLElement = document.getElementById("container");

const scrollbar: CreateScrollbar = createScrollbar();

scrollbar.attach(el);
```

## Parameters

### options?

#### activeThumbClassName?

`string` \| `false`

The class name for thumb active state in headless mode.

By default, it is disabled with `false`.

#### activeTrackClassName?

`string` \| `false`

The class name for track active state in headless mode.

By default, it is disabled with `false`.

#### disabled?

`boolean`

Whether disable the scrollbar.

By default, it is `false`.

#### headless?

`boolean`

Whether enable headless mode.

By default, it is `false`.

#### page?

`boolean`

Whether the scrollbar serve for a page.

By default, it is `false`.

#### setScrollbarLength?

(`length`) => `number`

Set the length of the scrollbar.

By default, it match with the default style.

#### x?

\{
  `activeThumbClassName?`: `string` \| `false`;
  `activeTrackClassName?`: `string` \| `false`;
  `onActive?`: (`options`) => `void`;
  `setScrollbarLength?`: (`length`) => `number`;
\}

Individual options for horizontal scrollbar.

#### x.activeThumbClassName?

`string` \| `false`

The class name for thumb active state in headless mode.

By default, it is disabled with `false`.

#### x.activeTrackClassName?

`string` \| `false`

The class name for track active state in headless mode.

By default, it is disabled with `false`.

#### x.onActive?

(`options`) => `void`

Triggered on scrollbar active state change.

#### x.setScrollbarLength?

(`length`) => `number`

Set the length of the scrollbar.

By default, it match with the default style.

#### y?

\{
  `activeThumbClassName?`: `string` \| `false`;
  `activeTrackClassName?`: `string` \| `false`;
  `onActive?`: (`options`) => `void`;
  `setScrollbarLength?`: (`length`) => `number`;
\}

Individual options for vertical scrollbar.

#### y.activeThumbClassName?

`string` \| `false`

The class name for thumb active state in headless mode.

By default, it is disabled with `false`.

#### y.activeTrackClassName?

`string` \| `false`

The class name for track active state in headless mode.

By default, it is disabled with `false`.

#### y.onActive?

(`options`) => `void`

Triggered on scrollbar active state change.

#### y.setScrollbarLength?

(`length`) => `number`

Set the length of the scrollbar.

By default, it match with the default style.

## Returns

[`CreateScrollbar`](../type-aliases/CreateScrollbar.md)
