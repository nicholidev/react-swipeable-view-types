# Installation
> `npm install --save @types/react-swipeable-view`

# Summary
This package contains type definitions for react-swipeable-view (https://github.com/oliviertassinari/react-swipeable-view).

# Details
Files were exported from https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/types/react-swipeable-view.
## [index.d.ts](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/types/react-swipeable-view/index.d.ts)
````ts
// Type definitions for react-swipeable-view 0.13
// Project: https://github.com/oliviertassinari/react-swipeable-view
// Definitions by: Michael Ledin <https://github.com/mxl>
//                 Deividas Bakanas <https://github.com/DeividasBakanas>
// Definitions: https://github.com/DefinitelyTyped/DefinitelyTyped
// TypeScript Version: 2.8

import * as React from 'react';

export type OnChangeIndexCallback = (index: number, indexLatest: number) => void;

export type OnTransitionEndCallback = () => void;

export type OnSwitchingCallback = (index: number, type: OnSwitchingCallbackTypeDescriptor) => void;

export type OnSwitchingCallbackTypeDescriptor = "move" | "end";

export type AxisType = "x" | "x-reverse" | "y" | "y-reverse";

export interface SpringConfig {
    duration: string;
    easeFunction: string;
    delay: string;
}

export interface SwipeableViewsProps extends React.HTMLProps<HTMLDivElement> {
    animateHeight?: boolean | undefined;
    animateTransitions?: boolean | undefined;
    axis?: AxisType | undefined;
    containerStyle?: React.CSSProperties | undefined;
    disabled?: boolean | undefined;
    /*
     * This is the config used to disable lazy loading, if true it will render all the views in first rendering.
     */
    disableLazyLoading?: boolean | undefined;
    enableMouseEvents?: boolean | undefined;
    hysteresis?: number | undefined;
    ignoreNativeScroll?: boolean | undefined;
    index?: number | undefined;
    onChangeIndex?: OnChangeIndexCallback | undefined;
    onSwitching?: OnSwitchingCallback | undefined;
    onTransitionEnd?: OnTransitionEndCallback | undefined;
    resistance?: boolean | undefined;
    style?: React.CSSProperties | undefined;
    slideStyle?: React.CSSProperties | undefined;
    springConfig?: SpringConfig | undefined;
    slideClassName?: string | undefined;
    threshold?: number | undefined;
}

export interface SwipeableViewsState {
    indexCurrent?: number | undefined;
    indexLatest?: number | undefined;
    isDragging?: boolean | undefined;
    isFirstRender?: boolean | undefined;
    heightLatest?: number | undefined;
    displaySameSlide?: boolean | undefined;
}

export default class SwipeableViews extends React.Component<SwipeableViewsProps, SwipeableViewsState> { }

````

### Additional Details
 * Last updated: Wed, 07 Jul 2021 18:31:45 GMT
 * Dependencies: [@types/react](https://npmjs.com/package/@types/react)
 * Global values: none

# Credits
These definitions were written by [Michael Ledin](https://github.com/mxl), and [Deividas Bakanas](https://github.com/DeividasBakanas).
