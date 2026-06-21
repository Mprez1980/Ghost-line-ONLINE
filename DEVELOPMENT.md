# Ghost-line ONLINE - Development Guide

## Getting Started

This is a static website project with e-commerce integration planned for the future.

### Current Tech Stack
- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Hosting**: GitHub Pages (coming soon)
- **E-Commerce**: [TBD - Gumroad/Lemonsqueezy recommended]
- **Illustrations**: SVG + Procreate/Adobe Illustrator
- **Animations**: CSS3 Animations + GSAP.js
- **Community**: Discord embed or GitHub Discussions
- **Video**: YouTube embed integration

### Project Structure

```
src/
├── index.html          # Main homepage
├── css/
│   ├── style.css       # Global styles
│   ├── factions.css    # Faction-specific styles
│   ├── animations.css  # Animation library
│   └── responsive.css  # Mobile-first design
├── js/
│   ├── interactive.js  # Interactive elements
│   ├── animations.js   # GSAP animations
│   ├── faction-selector.js
│   └── video-gallery.js
└── assets/
    ├── images/
    ├── illustrations/
    │   ├── characters/
    │   ├── factions/
    │   └── symbols/
    ├── symbols/
    └── audio/

pages/
├── factions/
│   ├── union.html
│   ├── necromancers.html
│   ├── contextualists.html
│   ├── yesteryear.html
│   └── conclave.html
├── characters.html
├── story.html
├── community.html      # NEW: Community forum/Discord
├── media.html          # NEW: Videos, trailers, podcasts
├── store.html
└── interactive.html

docs/
├── worldbuilding/
├── characters/
└── themes.md

media/
├── videos/
│   ├── trailers/
│   ├── tutorials/
│   └── lore-videos/
├── podcasts/           # Coming soon
└── artwork/
```

## Development Workflow

### 1. Local Testing
- Clone the repository
- Open `src/index.html` in a browser
- Make changes and test locally

### 2. Creating New Pages
- Create new HTML file in appropriate folder
- Use existing pages as template
- Link from navigation and relevant pages

### 3. Adding Content
- Faction documentation goes in `docs/worldbuilding/`
- Character profiles in `docs/characters/`
- HTML pages go in `pages/` folder

## Branches

Use feature branches for new work:

```bash
git checkout -b feature/faction-pages
git checkout -b feature/character-profiles
git checkout -b feature/illustrations
git checkout -b feature/animations
git checkout -b feature/community-forum
git checkout -b feature/video-gallery
git checkout -b feature/e-commerce
git checkout -b feature/interactive-quiz
```

## Next Steps

### Phase 1: Foundation
- [ ] Set up GitHub Pages
- [ ] Create all faction detail pages
- [ ] Create character profile pages
- [ ] Finalize lore documentation
- [ ] Set up basic animations library

### Phase 2: Visual Design & Illustrations
- [ ] Commission/create faction character illustrations
- [ ] Design faction symbol logos (SVG)
- [ ] Create atmospheric background illustrations
- [ ] Design UI elements and icons
- [ ] Add CSS animations (fade-ins, transitions, hovers)

### Phase 3: Interactivity & Media
- [ ] Build faction quiz with animations
- [ ] Create interactive timeline (animated)
- [ ] Implement quote library
- [ ] Add animations and transitions
- [ ] Set up video gallery page
- [ ] Create YouTube embed integration
- [ ] Add video playlists by faction/theme

### Phase 4: Community & E-Commerce
- [ ] Set up Discord server (embed on community page)
- [ ] Or enable GitHub Discussions
- [ ] Set up Gumroad/Lemonsqueezy account
- [ ] Create first ebook product
- [ ] Add store page with embedded cart
- [ ] Set up payment processing

### Phase 5: Expansion
- [ ] Build interactive apps
- [ ] Create merchandise
- [ ] Launch podcast (audio content)
- [ ] Add user accounts and wishlists
- [ ] Consider custom store platform

## Assets Needed

### Illustrations
- [ ] Character portraits (Wisp, Aster, Rook, Vale founders)
- [ ] Faction leader illustrations
- [ ] Action scenes (conflict, collaboration)
- [ ] Environment/world art
- [ ] Faction-specific aesthetics (The Union = heavenly, Necromancers = ancient Egypt/metal, etc.)
- [ ] Icon set for UI

### Animations
- [ ] Page load transitions
- [ ] Faction hover effects
- [ ] Scrolling parallax effects
- [ ] Character reveal animations
- [ ] Quote rotation animations
- [ ] Button interactions
- [ ] Modal pop-ups
- [ ] Timeline progression animations

### Video Content
- [ ] Animated trailers (faction introductions)
- [ ] Character origin stories
- [ ] World-building documentaries
- [ ] Behind-the-scenes creation content
- [ ] Lore explanations
- [ ] Fan art showcases

### Audio
- [ ] Ambient background music by faction
- [ ] Theme songs
- [ ] Sound effects
- [ ] Podcast intro/outro

## Illustration Style Guide

### The Union
- **Colors**: Gold, white, blue, light pastels
- **Style**: Ethereal, glowing, heavenly
- **Themes**: Halos, light rays, angelic figures, religious iconography
- **Inspiration**: Renaissance religious art, stained glass

### The Necromancers
- [ ] **Colors**: Black, dark purple, blood red, gold accents
- **Style**: Dark, mystical, ancient
- **Themes**: Egyptian hieroglyphics, tribal patterns, skeletal imagery, runes
- **Inspiration**: Ancient Egypt, heavy metal album art, gothic aesthetics

### The Contextualists
- **Colors**: Deep teal, silver, warm earth tones
- **Style**: Sleek, sophisticated, hidden power
- **Themes**: Silhouettes, shadowy figures, glowing networks
- **Inspiration**: Corporate sci-fi, spy thrillers, hidden complexity

### Yesteryear (Terrorists)
- **Colors**: Neon 80s (bright pink, cyan, purple)
- **Style**: Retro-futuristic, chaotic
- **Themes**: 80s nostalgia, digital decay, cassette aesthetics
- **Inspiration**: 1980s VHS, synthwave, vaporwave

### The Conclave (Corporate)
- **Colors**: Sterile white, cold grays, corporate blues
- **Style**: Clean, corporate, clinical
- **Themes**: Circuits, data streams, control
- **Inspiration**: Tech corporations, dystopian sci-fi

## Animation Library

### CSS Animations to Implement
```css
/* Fade in on scroll */
.fade-in { animation: fadeIn 0.8s ease-in; }

/* Slide animations */
.slide-left { animation: slideLeft 0.6s ease-out; }
.slide-right { animation: slideRight 0.6s ease-out; }

/* Glow effect (faction-specific) */
.glow-union { animation: glowUnion 2s ease-in-out infinite; }
.glow-necro { animation: glowNecro 2s ease-in-out infinite; }

/* Parallax scrolling */
.parallax { background-attachment: fixed; }

/* Interactive hover effects */
.faction-card:hover { transform: scale(1.05); }
```

### JavaScript Animation Libraries
- **GSAP.js**: Advanced timeline animations
- **AOS (Animate On Scroll)**: Element reveal animations
- **Three.js**: 3D effects (optional future enhancement)

## Community Forum Options

### Option 1: Discord Embed (Recommended for MVP)
- Create Discord server
- Embed Discord widget on community page
- Easy moderation and engagement
- **Pros**: Free, community management tools, voice chat
- **Cons**: Off-site

### Option 2: GitHub Discussions
- Built into repository
- Integrated with your GitHub account
- **Pros**: Integrated, free, good for tech-focused community
- **Cons**: Less engaging UX

### Option 3: Custom Forum (Future)
- Discourse, Vanilla Forums, or custom build
- Full control and branding
- **Pros**: Branded, owned experience
- **Cons**: Requires backend, moderation overhead

**Recommendation**: Start with Discord for launch, migrate to custom later if needed.

## Video Integration

### YouTube Playlist Strategy
1. **Faction Introductions** (1-2 min each)
   - The Union's mission
   - Necromancers' philosophy
   - Contextualists' hidden work
   - etc.

2. **Character Stories** (3-5 min each)
   - Wisp's origins
   - Aster's journey
   - Rook's awakening
   - Vale company history

3. **World-Building** (5-10 min each)
   - The 300-year timeline
   - AI emergence explained
   - Crystalline technology deep dive
   - Emergence event origins

4. **Community Content** (various lengths)
   - Fan art showcases
   - User stories
   - Behind-the-scenes creation
   - Live Q&As

### Video Page Structure
```html
<div class="video-gallery">
  <div class="playlist">
    <h2>Faction Trailers</h2>
    <div class="video-grid">
      <!-- YouTube embeds -->
    </div>
  </div>
  
  <div class="playlist">
    <h2>Character Stories</h2>
    <!-- More embeds -->
  </div>
</div>
```

## E-Commerce Planning

### Product Ideas
- Faction Guide Ebook
- Complete Lore Bible
- Character Development Guide
- Timeline Poster (digital + physical)
- Interactive Quiz App
- Soundtrack (music by faction)
- Art Book (illustrations)
- Limited Edition Digital Assets
- Merchandise (physical: shirts, hoodies, posters)

### Platform Decision
- **Gumroad**: Simple, creator-friendly, good for getting started
- **Lemonsqueezy**: Good for products and apps, affiliate program
- **Stripe**: Full control but requires backend setup

**Recommendation**: Start with Gumroad for MVP, migrate to custom if needed.

## Collaboration

Guidelines for contributors:
- Use descriptive commit messages
- Create feature branches off main
- Test locally before pushing
- Update documentation as you add features
- Keep commits atomic and focused

## Resources

### Documentation
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Gumroad Documentation](https://help.gumroad.com/)
- [Web Accessibility Guidelines](https://www.w3.org/WAI/)
- [Markdown Guide](https://www.markdownguide.org/)

### Animation Libraries
- [GSAP Documentation](https://gsap.com/)
- [AOS (Animate On Scroll)](https://michalsnik.github.io/aos/)
- [Three.js](https://threejs.org/) (3D)

### Design Tools
- [Figma](https://www.figma.com/) (UI/UX design)
- [Adobe Illustrator](https://www.adobe.com/products/illustrator.html) (vector art)
- [Procreate](https://procreate.art/) (iPad illustration)
- [Aseprite](https://www.aseprite.org/) (pixel art)

### Media
- [YouTube Embed Generator](https://www.embed-code.com/)
- [Discord Widget](https://discord.com/developers)

## Questions?

Check the project issues or create a new one with questions or suggestions!
