This document is a rulebook for UI theming at Audentio. All new projects (mock-ups included) must follow this guideline, including non-react projects.

## Rules

1. All themable style propreties should follow the structure and naming convention defined below. 
2. Should you need a new value (this should be done very rarely), you must add to theme.
3. Do not use arbitrary values if that property-type exists in the theme.
  - e.g. fontSizes exist in theme so every font-size definition should come from theme.
4. To avoid useTheme calls for trivial things, import the theme as a static object and use that. 
  - This should **not** be done in projects that need theming at runtime.

## structure & naming

#### Font sizes

1. smallText
2. bodyText
3. paragraphTitle
4. sectionTitle
5. sectionSubtitle
6. heroTitle


#### Colors

Base:
- rootBackground
- background
- surface
- text
- mutedText
- faintText
- boldText
- border
- boldBorder

States (+shades)
- error
- danger - alias
- success
- info
- warning

Brand (+shades) 
- primary
- secondary
- tertiary