# Andy's Smart Tool Swapper 0.2.2

A fix for menus that showed no current values.

- **Fixed: every setting's current value rendered as blank space.** The value sat on a second line in light grey, and Bedrock draws form buttons on a light grey plate, so it was invisible. Buttons were two rows tall with an empty second row, which looked like a layout fault rather than a colour one. Secondary button text is now dark grey and reads clearly.
- The Back and Close buttons were affected the same way and are now legible.
- Nothing behavioural changed. Values were always stored and applied correctly; they simply could not be read.
