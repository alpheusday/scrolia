## 0.4.1

### What's Changed

- Avoid `NaN` value to be passed to CSS style property

## 0.4.0 (2025-04-17)

### Breaking Changes

- Remove `PageScrollbar` and `ComponentScrollbar` component
- Move options:
    - `disabled`
- Remove options:
    - `position`
    - `color`
    - `colorHover`
    - `colorActive`
    - `containerProps`
    - `contentProps`
    - `trackXProps`
    - `trackYProps`
    - `thumbXProps`
    - `thumbYProps` 
- Remove `useDeviceEnvironment` hook

### What's New

- Add components:
    - `Container`
    - `Content`
    - `TrackX`
    - `TrackY`
    - `ThumbX`
    - `ThumbY`
    - `Scrollbar`
- Add `page` option
- Add `headless` option
- Add `setScrollbarLength` option
- Add `activeTrackClassName` option
- Add `activeThumbClassName` option
- Add `x` object option
- Add `y` object option
- Add sourcemap support

### Migrating from 0.3.0 to 0.4.0

For page scrollbar:

```diff
import type * as React from "react";

- import { PageScrollbar } from "@scrolia/react";
+ import { Scrollbar } from "@scrolia/react";

const App = (): React.JSX.Element => {
    return (
        <>
-           <PageScrollbar>
+           <Scrollbar page>
                <div>Content</div>
-           </PageScrollbar>
+           </Scrollbar>
        </>
    );
}
```

For component scrollbar:

```diff
import type * as React from "react";

- import { ComponentScrollbar } from "@scrolia/react";
+ import { Scrollbar } from "@scrolia/react";

const Component = (): React.JSX.Element => {
    return (
        <div>
-           <ComponentScrollbar>
+           <Scrollbar>
                <div>Content</div>
-           </ComponentScrollbar>
+           </Scrollbar>
        </div>
    );
}
```

## 0.3.0 (2024-12-18)

### Breaking Changes

- Remove `enable` prop, use `disabled` prop instead
- Rename `colorDrag` to `colorActive`
- Update `useDeviceEnvironment` hook for the new prop

### What's New

- Add `disabled` prop
- Component now require the CSS to be imported

## 0.2.2 (2024-12-10)

### What's Changed

- Fix on the scrollbar update function
- Remove unused track and thumb on specific position

## 0.2.1 (2024-12-01)

### What's Changed

- Fix on styling
- Better support for the scrollbar on navigation
- Performance optimization

## 0.2.0 (2024-11-28)

### What's New

- Add support for ES Module
- Add `useDeviceEnvironment` hook
- Add `enable` option

### What's Changed

- Support all environments by default

## 0.1.1 (2024-05-30)

### What's Changed

- Fix the issue that the scrollbar do not update after popstate
- Avoid update on popstate event in same URL
 
## 0.1.0 (2024-05-30)

First release
