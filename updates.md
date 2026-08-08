
> **Fix the responsive issues in the wedding invitation footer without changing the existing design.**
>
> **Current Issues:**
>
> * On smaller screens, the **Play Music** button overflows outside the `.invitation-footer`.
> * The footer items do not share the available width equally.
> * The music button (`.music-note`) is positioned absolutely outside the footer instead of being part of the third `.invitation-footer-item`.
> * The layout breaks on mobile because the footer relies on fixed spacing and does not resize gracefully.
>
> **Requirements:**
>
> * Move the **Play Music** button inside the third `.invitation-footer-item`.
> * Use Flexbox so all three footer items (Venue, View Map, Play Music) occupy equal space.
> * Add appropriate `flex`, `min-width: 0`, and responsive sizing to prevent overflow.
> * Keep all text and icons vertically centered.
> * Maintain the existing pill-shaped footer design, colors, border radius, spacing, and typography.
> * Keep vertical separators between items on desktop, but hide them on mobile.
> * On screens below **480px**, either:
>
>   * keep all three items on one row by scaling text/icons appropriately, or
>   * wrap gracefully into two rows without any overflow.
> * Use `clamp()` for responsive font and icon sizes.
> * Avoid fixed widths wherever possible.
> * Ensure the footer never exceeds the width of its parent container.
> * Preserve accessibility and existing functionality of the music player.
>
> **Expected Result:**
>
> * The footer remains fully responsive from desktop to mobile.
> * No content overflows outside the footer.
> * Equal spacing between Venue, View Map, and Play Music.
> * Clean, balanced layout consistent with the invitation design.
