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
Sydney, Australia · [boblee.dev](https://www.boblee.dev) · [Email](mailto:lb15058460816@gmail.com) · [LinkedIn](https://www.linkedin.com/in/bob-lee-433011356/))

Most software asks to be noticed. I’m interested in the opposite: interfaces that leave room to think, systems whose structure stays legible as they grow, and details whose charm comes from how they work.

Open to frontend and full-stack internships in Sydney.


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
