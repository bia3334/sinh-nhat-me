# Thiệp sinh nhật Mẹ — rules for AI agents

One self-contained page, `index.html`, for the owner's mother's birthday (30/10/2026).
Live at https://bia3334.github.io/sinh-nhat-me/ — GitHub Pages from `main` root, so
`git push origin main` = deploy.

- **Vietnamese only.** Every visible word is hardcoded in the markup so the owner edits
  it in place. The `CÀI ĐẶT` script block holds only what JS needs (`NHAC`, `HOA_BAY`,
  the two mic status strings). Fonts (Great Vibes + Alegreya, latin + vietnamese
  subsets) are base64 in the bottom `<style>` — don't touch.
- **The owner hand-edits `index.html`.** Make targeted edits only; never regenerate or
  overwrite the file wholesale.
- **The letter** (`✉️ VIẾT THƯ Ở ĐÂY`) is in the owner's plain voice: no invented
  memories, metaphors or feelings. Mẹ is a quân nhân (Thượng tá); the voice is con–Mẹ,
  warm and respectful.
- The letter links to the graduation pages of Mẹ / Ba / Đạt with `?m=<ddmmyyyy>`
  (30101975, 01011973, 07042007) so they open in letter mode — one tap "Mở xem", no DOB
  typing. If a DOB changes in `graduation/guests/*.html`, update these links.
- Flow: dark room, candle-lit cake → "Thổi nến" button / tap the cake / blow into the mic
  → candles out, smoke, a beat of darkness → lights on: flowers burst from the cake,
  bunting, balloons, music-box birthday tune (Web Audio, unlocked inside the click), and
  an orange tabby trots back and forth along the bottom (tap → stops, hops, "Meo meo~")
  → scroll: the folded card's cover flips up, more flowers fly out, letter revealed.
  "Thắp nến lại" replays it. Mẹ likes cats and flowers — the owner asked for both.
- `anh-xem-truoc.png` is the `og:image` (1200×630, lit hero) for the Zalo/Messenger
  link preview.
- Check visually with Chrome headless before shipping. Headless doesn't advance CSS
  transitions or `requestAnimationFrame`, so force the end state by injecting
  `class="thoi sang"` on `<html>` plus `*{transition:none!important}`; to see the flowers
  fly, stub `requestAnimationFrame` with a 16 ms `setTimeout` before the page script.
