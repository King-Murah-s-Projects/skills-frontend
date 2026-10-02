# Interface Method

## Layout

Use the structure that fits the work:

- Tables for desktop comparison and scanning.
- Cards for mobile equivalents of list rows.
- Drawers or side panels for record detail when users need to return to a list.
- Dialogs for focused confirmation, reason capture, and short forms.
- Full pages for workflows that need room, navigation, or durable URL state.

Avoid nested cards, decorative shells, and hero-style layouts in operational tools. Do not put cards inside cards unless the local design system already does it for a specific reason.

## Controls

Use familiar controls:

- Inputs for free text.
- Selects, menus, segmented controls, or tabs for option sets.
- Checkboxes or switches for binary settings.
- Tables or structured rows for comparison.
- Buttons for commands.
- Icon buttons only when the icon is familiar or a tooltip/label is available.

Maintain stable dimensions for controls, rows, cards, boards, and toolbars so dynamic labels, hover states, loading text, and icons do not resize the layout.

## Accessibility

At minimum:

- Use semantic buttons, links, labels, tables, headings, lists, and status regions.
- Keep focus visible and restore focus when drawers/dialogs close.
- Give icon-only controls an accessible name.
- Use text plus color or icon for statuses.
- Keep important controls at practical touch-target sizes, usually 44px or more.
- Announce meaningful loading, error, success, stale, and empty states.
- Check keyboard activation for critical actions.

## Responsive Behavior

Verify that text fits its container and does not overlap at mobile and desktop widths.

For list workspaces, desktop tables and mobile cards should present equivalent data and actions. Pagination, result ranges, filters, and selected detail should remain understandable on both.

## Visual System

Use the project's tokens and primitives:

- Avoid raw color and font values when semantic tokens exist.
- Keep status, warning, success, danger, and brand colors semantically separate.
- Use the installed icon library.
- Use typography scale intentionally: large type for true page hierarchy, compact type for dense tools.
- Do not let a one-note palette dominate unless the brand or project explicitly requires it.
