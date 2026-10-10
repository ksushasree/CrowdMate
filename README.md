# CrowdMate AI – Smart Stadium Management

Single-file website. Open `index.html` in any modern browser (no build step, no dependencies).

## Connecting live data
Edit the `CONFIG` object near the top of the `<script>` in `index.html`:
- `endpoints`: gates, parking, alerts, scores, matches, menu (JSON GET URLs)
- `orders`: POST URL for food orders
- `ai`: POST URL for an AI assistant ({message, context} -> {reply})
The expected JSON shape for each is documented in the comment above `CONFIG`.

Match selection, cart, seat, orders and chat are saved in the browser (localStorage).
