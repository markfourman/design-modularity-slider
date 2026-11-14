# Integrated or modular? A 3D supply chain trade-off slider

**Live link:** https://markfourman.github.io/integrated-vs-modular-slider/

Pick a product, then drag one slider from integrated (one sealed design) to modular (standard, swappable parts). A 3D model of the product comes apart as you go, and the flexibility, cost and benefit scores update live. It covers five products: a desktop PC, furniture, a smartphone, a bicycle and kitchen cabinets. Each one has three real examples on the slider, with sources.

![The app showing a desktop PC taken apart into its modules, with a flexibility score of 10 out of 10 and 96 configurations](screenshot.png)

## What the slider teaches

The more modular a product is, the more flexible it is, for the customer and for the company. That flexibility has a price.

- **Choices multiply. Parts only add.** Four modules with 4, 3, 2 and 4 options make 4 × 3 × 2 × 4 = 96 products from 4 + 3 + 2 + 4 = 13 kinds of part. A modular maker can offer a lot of variety without stocking a lot of different finished products.
- **Shared parts lower inventory risk.** One stock of common parts can be turned into whichever product is ordered. This is called risk pooling.
- **Final assembly can wait.** If the product is finished only after the real order arrives, less has to be guessed in advance. This is called postponement.
- **It is a trade-off, not a verdict.** Modular designs take more design work and more parts to manage. Unit cost can go either way: sealing parts in is the cheap end for electronics, and flat-pack is the cheap end for furniture.

## How to use it

1. Pick a product with the buttons at the top.
2. Drag the slider from Integrated to Modular, or tap one of the three names under it to jump to a real example.
3. Read the scores as they change. Drag the 3D model to turn it, and tap a part to see what it is.

Other things you can do:

- **Compare all three** shows the three real examples side by side.
- **Save this view** downloads a 1200 × 630 picture of the model and scores, sized for a LinkedIn post.
- **Copy LinkedIn post** copies a short draft post for the product and slider position you are on.
- Tap any word with a dotted underline for a plain definition.

## Compatibility

- One file, no build step, no typing anywhere. Works with touch, mouse and keyboard (arrow keys move the slider).
- The 3D view uses Three.js (r128) loaded from a CDN, with WebGL.
- If WebGL is switched off or the CDN is blocked, as on some work laptops, the page switches to a built-in basic 3D view. Everything else works the same, and the page shows a small "Basic 3D mode" note.
- Fonts (Barlow) come from Google Fonts. If they are blocked, the page falls back to system fonts.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The whole app: HTML, CSS and JavaScript in one file |
| `preview.png` | The picture that shows when the link is shared (1200 × 630) |
| `screenshot.png` | The screenshot used in this README |
| `linkedin-post.md` | A launch post draft, plus a three-sentence version |

## Publishing on GitHub Pages

1. Create a public repository named `integrated-vs-modular-slider`.
2. Upload `index.html`, `preview.png`, `screenshot.png` and `README.md` to the main branch.
3. In the repository, open Settings, then Pages. Under "Build and deployment", choose "Deploy from a branch", pick `main` and `/ (root)`, and save.

The page goes live at the link above after a minute or two. The link preview and the "Copy LinkedIn post" button both use that address, so keep the repository name as it is.

## Which figures are illustrative and which are sourced

**Illustrative (judgments made for teaching, not measurements):**

- Every score: flexibility out of 10, and the three cost scores and four benefit scores out of 5. Each has its reason printed beside it.
- The number of options per module (for example 3, 4, 2 and 4) and the totals that follow from them (96 configurations, 13 kinds of part). The totals are plain arithmetic on the example numbers.
- Scores between two anchors. They are blended in a straight line from the two nearest anchors.
- The 3D models. They are simple teaching models, not drawings of real products.

**Sourced (each has a citation in the app and in the references below):**

| Claim in the app | Source |
| --- | --- |
| Mac mini memory is part of the chip package and can't be upgraded after purchase | Apple (2026a) |
| Dell desktops: storage, memory and often graphics can be upgraded; upgrade motherboards are generally not available | Dell (2026) |
| Framework Desktop: standard Mini-ITX board, swappable front port cards, soldered memory | Framework (2025) |
| West Bros Furniture, Hanover, Ontario: glued mortise and tenon joints | Hofmann (2026) |
| Canadel: Canadian-made custom dining furniture; production lead time of 4 to 6 weeks for new orders | Canadel (n.d.) |
| IKEA's 1953 catalogue had three flat-pack tables; flat packs fit far more product into trucks and warehouses | IKEA Museum (n.d.) |
| iPhone: genuine parts are sold; the repair manual is for experienced technicians and uses a heated fixture to soften display adhesive | Apple (2026b) |
| Galaxy XCover7 Pro: user-replaceable battery | Samsung (n.d.) |
| Fairphone (Gen. 6): up to 12 spare parts owners can replace; a single screwdriver opens the phone | Fairphone (n.d.) |
| VanMoof: battery, main board and electronic shifter fit inside the frame | Schmitz (2023) |
| VanMoof declared bankrupt on 17 July 2023; spare parts and repair bookings stopped | Croxton (2023) |
| Giant D-Fuse seatpost: D-shaped, fits only selected Giant and Liv bikes | Giant Bicycles (n.d.) |
| Surly Steamroller: sold as a frame and fork only, with a 68 mm threaded shell for the crank bearings | Surly Bikes (n.d.) |
| Custom cabinets: built by hand, delivery up to nine or more weeks. Semi-custom: longer lead time than stock. Stock: often the same day or within a few days | The Home Depot Canada (n.d.) |
| KraftMaid: semi-custom; cabinet widths start at 6 inches and go up in 3-inch steps | KraftMaid (2022) |
| IKEA SEKTION: cabinets in a range of heights, widths and depths, with fronts and interior fittings chosen separately | IKEA Canada (n.d.) |

No market prices are used anywhere in the app.

**Worth checking yourself before you present it:**

- **Chapter number.** The app and this README cite Chapter 10 of Simchi-Levi et al. (2022) for "Coordinated Product and Supply Chain Design". McGraw Hill India's contents list for the 4th edition agrees. Two other listings (McGraw Hill Australia and a German bookseller) show it as Chapter 11, with a contents list that looks like the 3rd edition's. Check your own copy.
- **The 96 example.** The 4 × 3 × 2 × 4 = 96 example came from the project brief. It was not checked against the textbook, so the app presents it as an illustrative example and does not cite it to the book.
- **Journal articles.** For Fisher (1997), Feitzinger and Lee (1997) and Ulrich (1995), the journal, volume, issue and page numbers were checked against indexes. The app uses them for concepts only, not for figures.
- **Canadel's lead time.** The 4 to 6 weeks is a notice on Canadel's site that can change.
- **Samsung's spec page.** It lists the battery as user replaceable, which was confirmed against the specification table in Samsung's own news release for the phone.

All web sources were retrieved on November 14, 2026.

## References

- Apple. (2026a, September 21). *Upgrade or install memory in your Mac mini*. Apple Support. Retrieved November 14, 2026, from <https://support.apple.com/en-ca/102328>
- Apple. (2026b, October 23). *iPhone introduction* [Repair manual]. Apple Support. Retrieved November 14, 2026, from <https://support.apple.com/en-ca/125146>
- Canadel. (n.d.). *Canadel store in Ottawa*. Retrieved November 14, 2026, from <https://canadel.com/canadel-stores/ottawa/?lang=en>
- Croxton, J. (2023, July 19). *E-bike brand VanMoof declared bankrupt*. Cyclingnews. Retrieved November 14, 2026, from <https://www.cyclingnews.com/news/e-bike-brand-vanmoof-declared-bankrupt>
- Dell. (2026, October 9). *Upgrades to consider for your Dell computer* (Article No. 000191108). Dell Support. Retrieved November 14, 2026, from <https://www.dell.com/support/kbdoc/en-ca/000191108/upgrades-to-consider-for-your-dell-computer>
- Fairphone. (n.d.). *The Fairphone (Gen. 6)*. Retrieved November 14, 2026, from <https://www.fairphone.com/the-fairphone-gen-6>
- Feitzinger, E., & Lee, H. L. (1997). Mass customization at Hewlett-Packard: The power of postponement. *Harvard Business Review, 75*(1), 116–121.
- Fisher, M. L. (1997). What is the right supply chain for your product? *Harvard Business Review, 75*(2), 105–116.
- Framework. (2025, February 25). *Introducing the Framework Desktop* [Online forum post]. Framework Community. Retrieved November 14, 2026, from <https://community.frame.work/t/introducing-the-framework-desktop/65008>
- Giant Bicycles. (n.d.). *D-Fuse composite seatpost*. Retrieved November 14, 2026, from <https://www.giant-bicycles.com/au/d-fuse-composite-seatpost>
- Hofmann, A. (2026, May 25). *What makes quality wood furniture last?* West Bros Furniture. Retrieved November 14, 2026, from <https://www.westbrosfurniture.com/blogs/journal/what-makes-quality-wood-furniture-last>
- The Home Depot Canada. (n.d.). *How to buy kitchen cabinets: Buying guide*. Retrieved November 14, 2026, from <https://www.homedepot.ca/en/home/ideas-how-to/kitchen/how-to-buy-kitchen-cabinets.html>
- IKEA Canada. (n.d.). *How to choose kitchen cabinets and cabinet interiors*. Retrieved November 14, 2026, from <https://www.ikea.com/ca/en/rooms/kitchen/how-to/how-to-choose-kitchen-cabinets-and-cabinet-interiors-pubde8f91e0>
- IKEA Museum. (n.d.). *How IKEA took flatpacks to a whole new level*. Retrieved November 14, 2026, from <https://ikeamuseum.com/en/explore/the-story-of-ikea/flatpacks/>
- KraftMaid. (2022, June 23). *What are standard kitchen cabinet sizes?* Retrieved November 14, 2026, from <https://www.kraftmaid.com/kraftmaid/kitchen-cabinet-sizes>
- Samsung. (n.d.). *Galaxy XCover7 Pro: Specifications*. Samsung Mobile Press. Retrieved November 14, 2026, from <https://www.samsungmobilepress.com/media-assets/galaxy-xcover7-pro?tab=specs>
- Schmitz, R. (2023, August 23). *The downfall of e-bike company VanMoof has left its customers stranded* [Radio broadcast transcript]. NPR. Retrieved November 14, 2026, from <https://www.npr.org/2023/08/23/1195541570/the-downfall-of-e-bike-company-vanmoof-has-left-its-customers-stranded>
- Simchi-Levi, D., Kaminsky, P., & Simchi-Levi, E. (2022). *Designing and managing the supply chain: Concepts, strategies and case studies* (4th ed.). McGraw Hill.
- Surly Bikes. (n.d.). *Steamroller frameset*. Retrieved November 14, 2026, from <https://surlybikes.com/products/steamroller-frameset-anxious-lavender>
- Ulrich, K. (1995). The role of product architecture in the manufacturing firm. *Research Policy, 24*(3), 419–440.

## Credits

Built by [Mark Fourmanovskis](https://www.linkedin.com/in/mark-fourmanovskis/), a supply chain management student at Seneca Polytechnic. 3D drawing uses [Three.js](https://threejs.org/) (MIT licence).
