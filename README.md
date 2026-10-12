# Thought Radius

**How big can one mind be?** Only as wide as a signal can travel during one of its thoughts.

Thought Radius is a one-page calculator that accompanies the Medium article *There Will Never Be One Superintelligence* by Ed Daniels. Pick how fast a mind thinks, how far apart its parts are, and what carries its signals. The calculator tells you whether those parts can work as one mind, a team, a society, or a civilization.

It runs entirely in the browser. There's no login, no tracking, and nothing is stored.

**Live page:** `https://<your-username>.github.io/thought-radius/` (fill in after publishing)

## How to use it

- **Try:** preset scenarios from the article, including a GPU chip, your brain, one AI across Earth, and Mars at AI speed versus human speed.
- **How long does one thought take?** A slider from 1 nanosecond to 1 year, with quick picks. The *Think 1,000× faster* button shows the article's main point: speed shrinks minds.
- **How far apart are its parts?** A slider from 1 centimeter to about 10 light-years, with landmarks. You can also tap or drag on the ruler.
- **What carries the signals?** Light in space, optical fiber, or nerve fibers.

## How it works

A **thought** is one complete cycle in which a mind pulls in information from all of its parts, combines it, and settles on a result that becomes the starting point for the next cycle. What counts as one thought depends on the kind of mind: one chip cycle, one pass through an AI model, a moment of human perception, a considered decision. Richer thoughts are built from many of these cycles, and each one still needs every part to check in on time, so a mind's size is set by its shortest cycle that needs all of its parts.

The **thought radius** is how far a signal travels during one thought:

```
thought radius = signal speed × thought time
```

The calculator compares the distance between the mind's parts with that radius:

| Distance between parts | Verdict | Meaning |
|---|---|---|
| Up to 1/10 of the thought radius | One mind | Every part can join every thought. |
| 1/10 to 10 times the radius | A team | The parts must specialize and coordinate. |
| 10 to 10,000 times the radius | A society | Separate minds exchanging messages. |
| More than 10,000 times the radius | A civilization | Separate minds that share history, not thoughts. |

The one-tenth allowance for "one mind" reflects that a single thought needs many back-and-forth signals, and that real systems are slower than the ideal. The thresholds are judgment calls chosen to make the pattern visible. The pattern doesn't depend on them: faster thinking shrinks every zone, and no signal travels faster than light.

### Signal speeds

| Medium | Speed used | Notes |
|---|---|---|
| Light in space | 299,792 km/s | Radio and laser links between spacecraft |
| Optical fiber | About 200,000 km/s | Roughly two-thirds of light speed |
| Nerve fibers | 10 m/s | Slower long-range nerve fibers; real nerves range from about 1 to 120 m/s |

### Landmark distances

| Landmark | Distance used |
|---|---|
| Chip | 2.5 cm |
| Brain | 15 cm |
| Data center | 500 m |
| City | 30 km |
| Across Earth | 20,000 km (half the circumference) |
| Moon | 384,400 km |
| Mars | 225 million km (average; ranges from about 55 to 400 million km) |
| Voyager 1 | 25.9 billion km (one light-day, reached November 18, 2026) |
| Nearest star | 4.24 light-years (Proxima Centauri) |

## Publishing on GitHub Pages

1. Create a public repository named `thought-radius`.
2. Upload `index.html` and `README.md` to the repository root.
3. In **Settings > Pages**, set the source to **Deploy from a branch**, branch `main`, folder `/ (root)`.
4. After a minute or two the page appears at `https://<your-username>.github.io/thought-radius/`.
5. In `index.html`, replace `href="#"` on the article link (id `articleLink`) with the Medium URL once the article is live.

## Files

- `index.html`: the complete app. HTML, CSS and JavaScript in one file, with no build step and no dependencies. Atkinson Hyperlegible loads from Google Fonts, and the page falls back to system fonts if that fails.
- `README.md`: this file.

## Sources

- Sandberg, A. (1999). *The Physics of Information Processing Superobjects: Daily Life Among the Jupiter Brains.* https://simulation-argument.com/pdf/anders-sandberg-jupiter-brains.pdf
- Ringo, J. L., et al. (1994). *Time Is of the Essence: A Conjecture that Hemispheric Specialization Arises from Interhemispheric Conduction Delay.* Cerebral Cortex. https://doi.org/10.1093/cercor/4.4.331
- Bostrom, N. (2014). *Superintelligence: Paths, Dangers, Strategies.* Oxford University Press.
- Voyager 1 one light-day milestone: https://earthsky.org/space/voyager-1-1-light-day-from-earth-november-17-18-2026/

## Disclaimer

Concept by Ed Daniels. Calculator designed and built in collaboration with Claude. Ed Daniels claims ownership along with responsibility for any errors.
