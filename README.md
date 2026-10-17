# Bob Lee
<a href="https://www.boblee.dev">
  <img
    src="./miku_with_water.jpg"
    alt="Hatsune Miku touching a ripple that becomes the Oasis constellation"
    width="100%"
  >
</a>


**I build quiet software with a point of view.**

Computer Science at UNSW Sydney · Frontend / Full-stack  
Sydney, Australia · [boblee.dev](https://www.boblee.dev) · [Email](mailto:lb15058460816@gmail.com) · [LinkedIn](https://www.linkedin.com/in/bob-lee-433011356/)

Most software asks to be noticed. I’m interested in the opposite: interfaces that leave room to think, systems whose structure stays legible as they grow, and details whose charm comes from how they work.

Currently building [BuilderSpace](https://www.builderspace.dev), the website for a student builder community. Open to frontend and full-stack internships in Sydney.

---

## Selected work

### [Oasis](https://www.boblee.dev) — a digital garden that behaves like a place

Oasis is where I write, listen, and connect ideas: part publishing system, part music player, part knowledge map. I designed and built it end to end.

- **Motion, not vibration.** Its Live2D character moves from a smoothed attack–release envelope and beat phase rather than raw FFT values. The head leads; the body follows 180 ms later, turning audio data into movement with weight.
- **Coordinates with meaning.** Every post becomes a star whose angle encodes its creation date from the beginning of spring. Adding a new post never moves an old one, so the map can become familiar over time.
- **Chinese typography at the edge.** Social cards render arbitrary Chinese titles by requesting only the required glyphs for each title—a few kilobytes instead of shipping a complete multi-megabyte CJK font.
- **Useful when the network is not.** Supabase is the source of truth, while a local cache paints the first screen immediately and preserves the garden when cloud access fails.

`React 19` · `TypeScript` · `Tailwind CSS 4` · `Supabase` · `Cloudflare R2` · `Vercel Edge`

[Visit Oasis →](https://www.boblee.dev) · [View source →](https://github.com/BobLee-tech/Oasis)

---

### [BuilderSpace](https://www.builderspace.dev) — where student projects find their people

BuilderSpace is a bilingual builder community that started at UNSW. I built its site: a project plaza where members post what they are making and which roles they still need, then log progress until it ships. Chinese and English both render into the cached page, so switching language never refetches.

- **The database is the boundary.** There are no accounts and the browser only ever holds the anon key, so Postgres row-level security decides everything. Public submissions can only arrive as `pending`, sign-ups can be written but never read back, and rate limits live in database triggers rather than in the app.
- **Spam control that works from China.** Most CAPTCHAs do not load there, so forms use a honeypot and a fill-time check instead. Likely bots still see "success"; nothing reaches the database.
- **Operations without a CMS.** Organisers publish events, review projects and export sign-ups straight from Supabase. Triggers email them each new submission and a daily digest at 8 am Sydney time, with names only and never contact details. Comment moderation uses a passphrase checked inside Postgres against Vault and locks after repeated failures.
- **Chrome, not colour.** Black, white and liquid metal, drawn in raw WebGL with 1-bit Bayer dithering. The only colour is a 17,600-particle mascot sampled from the logo; it loads only when you scroll near it, drops resolution when the frame rate falls, and holds still under reduced motion.

`Next.js 16` · `React 19` · `TypeScript` · `Supabase` · `Postgres RLS` · `WebGL` · `Vercel`

[Visit BuilderSpace →](https://www.builderspace.dev) · [View source →](https://github.com/BobLee-tech/Bulidspace)

---

### Adaptiq — AI teaching software for tutoring centres

On a three-person team, I owned teacher reporting, student profiles, the administration console, and bilingual support. I also handled integration across 13 feature pull requests.

- Built a TypeScript AST check for untranslated interface copy, distinguishing missing translations from Chinese text that legitimately belongs in the source.
- Audited the API after multi-tenancy shipped and found a 374-line unauthenticated route that trusted a `student_id` supplied in the request body; removed the route and its exposed access path.
- Turned per-organisation module flags from a passive database column into server-enforced policy across 13 routes.

`Next.js` · `TypeScript` · `Supabase` · `Postgres RLS`

---

## Writing

I write long-form notes in Chinese about algorithms, software architecture, design, and learning—usually by taking an idea apart until I can explain why it works.

[Read the garden →](https://www.boblee.dev/#/garden)

---

TypeScript · React · Next.js · Node.js · PostgreSQL / Supabase · Tailwind CSS · Vercel

`#39C5BB` tends to find its way into everything I make.
