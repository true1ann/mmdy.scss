# MMDY.scss docs/introduction.md
## Controlling colors
There are two schemes for colors: `fill` and `outline`

> [!NOTE]  
> Dont expect every component to follow your preference, some components like `switch` or `segmented-buttons` wont follow your preference

| fill style | color             | class                    |
|------------|-------------------|--------------------------|
| fill       | primary           | `fill-primary`           |
| outline    | secondary         | `outline-secondary`      |
| fill       | primary-container | `fill-primary-container` |

and so on. `color` can be `[primary|secondary|tertiary|error]`, everything can support `-container` addition

> [!NOTE]  
> You ***MUST*** add one on every component. Some components like `sgemented-buttons` and `switches` will ignore your fill style.

> [!TIP]  
> Use fill styles to mark a secondary opinion, if you dont want to use `secondary` option for example. Correct usage of fill styles matters by case

### Usage
To actually change color mode of a component just append color mode's class, examlpes:
- `badge fill-primary`
- `alert outline-error`
- `fill-secondary button`

## Changing roundness
Currently you can change roundness of every side (`[top|bottom|left|right]`) but not the edges  
(Never saw a material you component with different corners on just one edge so i dont think those are needed)

| class         | action      |
|---------------|-------------|
| `br-X`        | all sides   |
| `br-top-X`    | only top    |
| `br-bottom-X` | only bottom |
| `br-left-X`   | only left   |
| `br-right-X`  | only right  |

> [!NOTE]  
> `X` means any value from [_variables.$borders](../scss/_variables.scss)

## Changing spacings
You can control padding and margins using these classes

| class        | action               |
|--------------|----------------------|
| `m-X`        | margin on all sides  |
| `p-X`        | padding on all sides |
| `m-top-X`    | margin on top        |
| `m-bottom-X` | margin on bottom     |
| `m-left-X`   | margin on left       |
| `m-right-X`  | margin on right      |
| `p-top-X`    | padding on top       |
| `p-bottom-X` | padding on bottom    |
| `p-left-X`   | padding on left      |
| `p-right-X`  | padding on right     |

> [!NOTE]  
> `X` means any value from [_variables.$spacings](../scss/_variables.scss)

## Controlling `display` property
You can toggle between `display` options with

| class            | action               |
|------------------|----------------------|
| `d-none`         | hide the element     |
| `d-block`        | display as block     |
| `d-inline`       | display inline       |
| `d-inline-block` | display inline-block |
| `d-flex`         | display as flex      |
| `d-grid`         | display as grid      |

## Flexbox utils
| class                 | action                               |
|-----------------------|--------------------------------------|
| `flex-row`            | set flex direction to row            |
| `flex-column`         | set flex direction to column         |
| `flex-row-reverse`    | set flex direction to row-reverse    |
| `flex-column-reverse` | set flex direction to column-reverse |
| `justify-content-X`   | control horizontal alignment         |
| `align-items-X`       | control vertical alignment           |

> [!NOTE]  
> `justify-content`'s X supports `[start|end|center|between|around|evenly]`

> [!NOTE]  
> `align-items`'s X supports `[start|end|center|baseline|stretch]`

## Controlling Width and Height
You can controll width and height using

| class | action     |
|-------|------------|
| `w-X` | set width  |
| `h-X` | set height |

> [!NOTE]  
> X is measured in % and can be any from 0 to 100

## Controlling grid
On a grid we have 12 columns

| class         | action           |
|---------------|------------------|
| `col-X`       | set column width |

> [!NOTE]  
> X can be any from 1 to 12