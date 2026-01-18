# SELFLESS — Music Video Production Guide
## Midjourney V7 | Beksiński Edition | Character Consistency System

---

# THE STORY

**"Selfless" = Becoming SELF-LESS (empty, no identity)**

THE SELF is an elongated, androgynous humanoid searching for their reflection in an infinite mirror labyrinth. Cold silver corridors stretch endlessly. But every mirror shows something wrong — not their face, but glimpses of an ochre organic world beyond the glass. THE OTHER is not a character but the environment itself: a living, breathing dimension of flesh-like architecture that watches, waits, and hungers.

Drawn by obsession, THE SELF steps through a mirror and enters this sepia world of impossible organic architecture. At first it's peaceful, beautiful, seductive — cathedral arches of ribbed tissue, towers of folded flesh, walls textured like stretched membrane. But the environment begins to consume them.

Their body begins to dissolve. Edges blur and fade. With each verse, the change creeps slowly — becoming translucent, fibrous, losing solidity. With each chorus, it accelerates violently — flesh unraveling into threads, body merging with the organic walls, identity dissolving into the environment.

THE SELF explores deeper, hoping to find themselves, but only loses more. The organic architecture shifts and morphs constantly — it IS the Other, surrounding them completely, absorbing them piece by piece.

In the climax, THE SELF finds one final mirror floating in the organic void. They look in and see the horror: they have BECOME a hollow silhouette, a fading outline filled with the environment's texture. Their old solid self is trapped IN the mirror, looking back, mouth open in silent scream. The watcher has become the watched. The consumed has become the consumer.

Desperate, the now-dissolving being reaches for the mirror, trying to touch their old self. But the strain unravels them completely. They fragment into wisps and threads, scattering into the void. The environment — THE OTHER — absorbs these remnants into its living walls.

Final image: the mirror floats alone in the organic cathedral void. Inside it, the trapped solid SELF presses against the glass forever. The environment pulses with slow breath. It has won. It has always won.

**The message:** When you give yourself completely to another, you don't just lose yourself — you become the thing that consumed you, and your true self becomes a prisoner you can never reach again.

---

# VISUAL STYLE: ZDZISŁAW BEKSIŃSKI

Every image must embody Beksiński's distinctive aesthetic:

| Element | Application |
|---------|-------------|
| **Color palette** | Ochre, sepia, amber, umber, dried blood browns, bone ivory |
| **Figures** | Elongated, stretched, distorted proportions |
| **Architecture** | Organic fading structures, impossible perspectives |
| **Atmosphere** | Dreamlike haze, soft edges, no clear horizon |
| **Lighting** | Diffuse, no clear source, volumetric fog |
| **Texture** | Oil painting quality, visible brushwork feel |
| **Mood** | Melancholic beauty, quiet horror, lonely vastness |

**CRITICAL:** Do NOT mix in other style descriptors (anime, cinematic, etc.). Pure Beksiński throughout.

---

# MIDJOURNEY V7 TIPS & TRICKS

## Parameter Cheat Sheet

| Parameter | Range | Recommended | Effect |
|-----------|-------|-------------|--------|
| `--s` (stylize) | 0-1000 | **400-500** | Higher = more artistic/creative, lower = more literal |
| `--c` (chaos) | 0-100 | **0-10** | Higher = more variation between generations |
| `--ow` (omni weight) | 0-1000 | **200-300** | Higher = stricter character adherence |
| `--sw` (style weight) | 0-1000 | **100** | Higher = stronger style reference influence |
| `--ar` | ratio | **16:9** | Aspect ratio (use 2:3 for portraits, 1:1 for faces) |
| `--seed` | number | varies | Lock randomness for reproducibility |
| `--no` | text | varies | Negative prompt (exclude elements) |

## Golden Rules for Consistency

### 1. Create Clean Reference Images First
- Generate references at **1024px** minimum
- Use **neutral expressions** (extreme expressions break identity)
- **Good lighting** - soft, diffuse, no harsh shadows
- **Simple backgrounds** - let the character be the focus

### 2. Ladder Angles Gradually
```
GOOD:  Front → 3/4 view → Mild profile → Hard profile
BAD:   Front → Hard profile (identity breaks)
```
Big angle jumps cause the most consistency failures.

### 3. Change ONE Variable at a Time
When iterating, only change one thing per generation:
- Angle OR lighting OR pose — not all three
- This helps identify what's causing issues

### 4. Save Seeds for Your "Home Base"
```
/imagine [prompt] --seed 12345
```
Once you get a good result, note the seed. Use it as your baseline for variations.

### 5. Use Vary (Region) for Fixes
If face is 80% right but nose/eyes drift:
1. Use **Vary (Region)** in Midjourney
2. Mask just the problem area
3. Regenerate without redrawing the whole scene

## Beksiński-Specific Prompt Tips

### Effective Keywords
```
Zdzislaw Beksinski style, ochre sepia palette, organic bone architecture,
dreamlike atmosphere, soft diffuse lighting, oil painting texture,
melancholic surrealism, impossible perspectives, decaying grandeur
```

### Enhance the Horror
- Add: `bone cathedral, ribcage arches, vertebrae columns`
- Add: `stretched membrane texture, dissolving flesh, hollow fading forms`
- Add: `foggy haze, no horizon, floating in void`

### Combine with Complementary Artists (Optional)
For variation, you can occasionally blend:
- `Beksinski and Giger` — more biomechanical
- `Beksinski and Frazetta` — more dynamic poses
- `Beksinski and Moebius` — cleaner lines

**But for this project, keep it PURE Beksiński for consistency.**

## Troubleshooting Common Issues

| Problem | Solution |
|---------|----------|
| Character looks different each time | Increase `--ow` to 300-400, use same reference angle |
| Image too literal/boring | Increase `--s` to 500-600 |
| Image too chaotic/abstract | Decrease `--s` to 300-400 |
| Style not matching reference | Increase `--sw` to 150-200 |
| Artifacts/distortion | Decrease `--ow` to 150-200 |
| Face drifting | Use Vary (Region) on face only |
| Figure not recognizable | Keep distinctive posture, add remnant cloth/wrappings |

## Workflow: Draft → Refine

**Step 1: Fast ideation**
```
[prompt] --draft --v 7
```
Draft mode is 10x faster, half the cost. Use it to test compositions.

**Step 2: Full quality winners**
Once you like a draft, regenerate without `--draft`:
```
[same prompt] --v 7 --s 450
```

**Step 3: Enhance if needed**
Use the **Enhance** button on draft jobs to polish them to full quality.

## Prompt Structure Best Practices

### Optimal Order
```
[Subject/Action], [Details], [Environment], [Style], [Technical params]
```

### Example Breakdown
```
Elongated humanoid figure standing in bone cathedral,     ← Subject
pale flesh with visible veins, hunched posture,          ← Details
vast ribcage arches surrounding, ochre sepia void,       ← Environment
Zdzislaw Beksinski style, oil painting texture,          ← Style
dreamlike atmosphere, soft diffuse lighting              ← Mood
--oref [URL] --ow 250 --sref [URL] --sw 100 --ar 16:9 --v 7 --s 450   ← Params
```

### Words Matter
| Instead of | Use |
|------------|-----|
| big | enormous, towering, vast, immense |
| scary | haunting, dreadful, ominous, foreboding |
| old | ancient, weathered, decayed, timeworn |
| dark | shadowed, murky, tenebrous, lightless |

Be specific. Vocabulary = better results.

## Seed Strategy for This Project

For maximum consistency across 90 images:

1. **Find a "master seed"** that produces good Beksiński atmosphere
2. **Use the same seed** for all environment-only shots
3. **For character shots**, let the seed vary but lock the `--oref`
4. **Document seeds** for any image you might want to revisit

---

# REFERENCE SYSTEM EXPLAINED

## V7 Reference Parameters

Midjourney V7 introduced **Omni Reference** (`--oref`) which replaces the V6 Character Reference (`--cref`). Here's what you need to know:

| Parameter | Version | What It Does | Weight Range | Default |
|-----------|---------|--------------|--------------|---------|
| `--oref [URL]` | **V7** | Omni reference - characters, objects, anything | `--ow 0-1000` | 100 |
| `--sref [URL]` | V6/V7 | Style reference - keeps aesthetic consistent | `--sw 0-1000` | 100 |
| `--cref [URL]` | V6 only | Character reference (deprecated in V7) | `--cw 0-100` | 100 |

### Recommended Settings for This Project

| Parameter | Recommended | Why |
|-----------|-------------|-----|
| `--ow` | **200-300** | Balanced character consistency without artifacts |
| `--sw` | **100** | Strong style adherence for Beksiński look |
| `--s` (stylize) | **400-500** | Sweet spot for artistic quality + prompt accuracy |
| `--v 7` | Always | Ensures V7 model |

### Combining References

```
prompt text --oref [char URL] --ow 250 --sref [style URL] --sw 100 --ar 16:9 --v 7 --s 450
```

**Important V7 Notes:**
- `--oref` costs **2x GPU time** compared to regular V7 images
- Cannot use `--oref` with Draft Mode or `--q 4`
- Keep `--ow` below 400 to avoid artifacts (unless using high `--s`)
- You can only use ONE image with `--oref` per prompt

## Reference Strategy Overview (STREAMLINED)

**THE SELF (5 character references — one per dissolution stage)**
- SELF-01: Intact solid (THE primary character, fully defined)
- SELF-02: Edges blurring (becoming translucent at edges, softening)
- SELF-03: Half-dissolved (fibrous texture, threads forming, merging)
- SELF-04: Hollow silhouette (mostly translucent, environment shows through)
- SELF-05: Fading remnant (wisps and traces, almost absorbed)

**THE OTHER (4 environment references)**
- ENV-MIRROR: Cold liminal labyrinth (silver-blue)
- ENV-PEACEFUL: Peaceful organic world (warm, inviting)
- ENV-AGGRESSIVE: Aggressive organic world (violent, consuming)
- ENV-APOCALYPSE: Dissolving environment (unraveling)

**Total: 9 reference images**

---

# STEP 1: CREATE CHARACTER REFERENCES (5 images)

Generate these FIRST. One image per dissolution stage. These are your consistency anchors.

---

## SELF-01: Intact Solid (PRIMARY CHARACTER)

**This is THE character. Generate multiple times until you love it.**

```
Elongated androgynous humanoid figure standing in void, unnaturally tall stretched proportions, pale ivory flesh with visible blue veins beneath translucent skin, sunken features neither male nor female, deep shadowed eye sockets with distant sorrowful gaze, arms slightly too long hanging at sides, hunched shoulders curved forward protectively, wearing tattered grey cloth wrappings that hang loosely, clearly defined edges and solid form, Zdzislaw Beksinski style, ochre sepia background, dreamlike atmosphere, soft diffuse lighting, melancholic surrealism, oil painting texture, full body view --ar 2:3 --v 7 --s 450
```

---

## SELF-02: Edges Blurring (Beginning Dissolution)

```
Same elongated androgynous humanoid now showing early dissolution, edges of body becoming soft and blurred, flesh taking on slightly translucent quality at extremities, fingertips and edges fading into atmosphere, features softening as if seen through fog, same hunched posture same tattered wrappings now fraying at edges, beginning to lose definition, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture, full body view --ar 2:3 --v 7 --s 450
```

---

## SELF-03: Half-Dissolved (Fibrous Transformation)

```
Same elongated humanoid now significantly dissolved, body becoming fibrous and thread-like in places, flesh unraveling into organic tendrils that drift outward, torso partially translucent showing internal textures like stretched membrane, one arm solid while other dissolves into flowing strands, form dissolving between solid features and dissolving wisps, same distinctive hunched posture, wrappings merging with dissolving form, Zdzislaw Beksinski style, brown ochre amber palette, dreamlike horror, oil painting texture, full body view --ar 2:3 --v 7 --s 500
```

---

## SELF-04: Hollow Silhouette (Mostly Dissolved)

```
Same elongated humanoid now mostly dissolved into hollow form, body a translucent silhouette with environment visible through, only outline and traces of internal structure remaining, flesh become like stretched gauze or membrane, figure like a fading photograph, same hunched posture preserved in ghostly outline, wisps and threads trailing from dissolving edges, Zdzislaw Beksinski style, figure semi-transparent against ochre void, dreamlike dissolution, oil painting texture, full body view --ar 2:3 --v 7 --s 450
```

---

## SELF-05: Fading Remnant (Almost Absorbed)

```
Elongated humanoid almost completely dissolved, barely visible outline of figure fragmenting into wisps and floating threads, form scattering into the atmosphere, same distinctive stretched proportions barely recognizable in fading traces, like smoke dispersing, final moments before complete absorption, fragments of former self drifting apart, Zdzislaw Beksinski style, fading figure against sepia darkness, oil painting texture, full body view --ar 2:3 --v 7 --s 450
```

---

# STEP 2: CREATE ENVIRONMENT REFERENCES (4 images)

---

## ENV-MIRROR: Cold Liminal Labyrinth

**Used for ACT 1 only — the cold world before entering the organic realm.**

```
Infinite corridor of mirrors stretching in all directions, cold silver-blue metallic surfaces, liminal backrooms aesthetic, impossible geometry, reflections multiplying into darkness, hints of warm ochre organic shapes bleeding through some mirror surfaces, cold clinical space being infected by organic wrongness, Zdzislaw Beksinski style, cold blue-silver palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture, unsettling emptiness, wide establishing shot, no figures --ar 16:9 --v 7 --s 400
```

---

## ENV-PEACEFUL: Peaceful Organic World

**Used for wonder, seduction, and calm verse moments.**

```
Vast serene landscape of organic flesh architecture, cathedral-like arches made of stretched membrane and sinew, towers of folded tissue rise in distance, walls textured like living skin, beautiful and inviting despite being made of flesh, gentle curves and organic flow, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture, no figures, wide establishing shot --ar 16:9 --v 7 --s 450
```

---

## ENV-AGGRESSIVE: Violent Organic World

**Used for choruses and intense transformation moments.**

```
Organic flesh architecture in violent aggressive motion, membrane-like structures stretching and tearing, tissue towers pulsing and reshaping, organic forms reaching and grasping hungrily, the environment actively consuming, walls of living tissue closing in threatening, aggressive organic movement, threatening alive architecture, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture, no figures, dynamic composition --ar 16:9 --v 7 --s 550
```

---

## ENV-APOCALYPSE: Dissolving Environment

**Used for final dissolution in ACT 5.**

```
Organic architecture in catastrophic dissolution, massive flesh structures unraveling into countless threads, wisps and tendrils flying in all directions, the environment destroying itself, tissue tearing apart, membrane arches dissolving, dust of disintegrating matter filling the air, dark umber fading to void black at edges, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture, no figures, extreme dissolution --ar 16:9 --v 7 --s 550
```

---

# REFERENCE URL TRACKING

After generating each reference image, paste its URL here:

```
CHARACTER REFERENCES (5 total):
[ ] SELF-01 (intact solid): https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1
[ ] SELF-02 (edges blurring): https://www.midjourney.com/jobs/dcf1f9be-66e4-47a1-b223-68f724d3a9ea?index=0&folder=selfless%20v1
[ ] SELF-03 (half-dissolved): https://www.midjourney.com/jobs/537bbea7-19a1-4e6e-8bfc-f52d487f4dcb?index=0&folder=selfless%20v1
[ ] SELF-04 (hollow silhouette): https://www.midjourney.com/jobs/c47b3f33-24a3-4366-943e-c35a9866b4c2?index=0&folder=selfless%20v1
[ ] SELF-05 (fading remnant): https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1

ENVIRONMENT REFERENCES (4 total):
[ ] ENV-MIRROR (cold labyrinth): https://www.midjourney.com/jobs/9f588892-6bb1-48ab-b40f-7d69a61e6fec?index=0&folder=selfless%20v1
[ ] ENV-PEACEFUL (peaceful organic): https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1
[ ] ENV-AGGRESSIVE (violent organic): https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1
[ ] ENV-APOCALYPSE (dissolving): https://www.midjourney.com/jobs/f9aa1070-27f1-4915-98b9-feb99001d014?index=0&folder=selfless%20v1
```

**Total: 9 reference images**

---

# ACT 1: THE MIRROR LABYRINTH (0:00 - 0:45)
*14 images — Slow discovery, building unease*

---

## Scene 1.1: Discovery (0:00 - 0:18) — 5 images

**1.1.1** — Wide establishing: figure in labyrinth

| OREF | SREF |
|------|------|
| SELF-01 | ENV-MIRROR |

```
Wide establishing shot, elongated humanoid figure stands small in center of infinite mirror corridor, cold silver-blue surfaces stretch in all directions, figure's warm flesh contrasts cold environment, searching posture, reflections multiply into distant darkness, Zdzislaw Beksinski style, liminal atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/9f588892-6bb1-48ab-b40f-7d69a61e6fec?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 350
```

---

**1.1.2** — Figure searching

| OREF | SREF |
|------|------|
| SELF-01 | ENV-MIRROR |

```
Medium shot, elongated pale figure walks through mirror corridor, three-quarter view, looking into each mirror passed with searching expression, arm reaching toward reflections, cold blue-silver environment, warm flesh tone figure, Zdzislaw Beksinski style, liminal atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/9f588892-6bb1-48ab-b40f-7d69a61e6fec?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 350
```

---

**1.1.3** — Looking into mirror (normal reflection)

| OREF | SREF |
|------|------|
| SELF-01 | ENV-MIRROR |

```
Over-shoulder shot, elongated figure stands before ornate mirror frame, reflection shows their own stretched form correctly, moment of peace, searching for self in reflection, cold corridor behind, Zdzislaw Beksinski style, liminal atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/9f588892-6bb1-48ab-b40f-7d69a61e6fec?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 350
```

---

**1.1.4** — First wrong reflection

| OREF | SREF |
|------|------|
| SELF-01 | ENV-MIRROR |

```
Close shot of mirror surface, reflection shows NOT the figure but glimpse of ochre organic shapes, organic architecture visible where face should be, warm sepia tones bleeding through cold silver glass, first sign something is wrong, Zdzislaw Beksinski style, dreamlike atmosphere, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/9f588892-6bb1-48ab-b40f-7d69a61e6fec?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**1.1.5** — Multiple wrong mirrors

| OREF | SREF |
|------|------|
| SELF-01 | ENV-MIRROR |

```
Wide shot mirror corridor, elongated figure walks between mirrors, every reflection shows glimpses of organic world instead of figure, ochre organic shapes in silver frames, warm sepia bleeding into cold blue environment, Zdzislaw Beksinski style, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/9f588892-6bb1-48ab-b40f-7d69a61e6fec?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

## Scene 1.2: The Watcher Revealed (0:18 - 0:32) — 5 images

**1.2.1** — Bone world in mirrors

| OREF | SREF |
|------|------|
| — | ENV-PEACEFUL |

```
Extreme close-up of mirror surface, reflection filled entirely with peaceful organic architecture, fleshy arches and tissue towers visible through glass, ochre sepia warmth inviting through cold silver frame, sense of vast world beyond, beautiful wrongness, Zdzislaw Beksinski style, dreamlike atmosphere, oil painting texture, no figure visible --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**1.2.2** — Figure notices

| OREF | SREF |
|------|------|
| SELF-01 | ENV-MIRROR |

```
Close-up elongated face, expression shifting from searching to confusion, eyes focused on mirror surface showing wrong reflection, first moment of awareness, beginning of fear, pale features lit by warm ochre glow from mirror, Zdzislaw Beksinski style, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/9f588892-6bb1-48ab-b40f-7d69a61e6fec?index=0&folder=selfless%20v1 --sw 100 --ar 1:1 --v 7 --s 400
```

---

**1.2.3** — Surrounded by watching

| OREF | SREF |
|------|------|
| SELF-01 | ENV-MIRROR |

```
Overhead wide shot, elongated figure stands at center of circular mirror chamber, every mirror surface filled with ochre organic world watching, figure small and alone surrounded by organic glimpses, trapped in observation, warm sepia pressing in from all sides, Zdzislaw Beksinski style, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/9f588892-6bb1-48ab-b40f-7d69a61e6fec?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**1.2.4** — The inviting mirror

| OREF | SREF |
|------|------|
| SELF-01 | ENV-PEACEFUL |

```
Medium shot, single large mirror glows with warm ochre light, beautiful peaceful organic landscape visible through glass like doorway, inviting seductive warmth, elongated figure drawn toward it hand reaching, seduction beginning, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**1.2.5** — Approaching threshold

| OREF | SREF |
|------|------|
| SELF-01 | ENV-PEACEFUL |

```
Medium tracking shot, elongated figure walks toward glowing mirror portal, organic world clearly visible through glass, warm ochre light illuminating pale flesh, leaving cold silver corridor behind, approaching point of no return, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

## Scene 1.3: The Crossing (0:32 - 0:45) — 4 images

**1.3.1** — Hand touches glass

| OREF | SREF |
|------|------|
| SELF-01 | ENV-PEACEFUL |

```
Extreme close-up, pale elongated hand presses against mirror surface, glass ripples like liquid at touch, organic world visible through distorting surface, moment before crossing, flesh meeting barrier to other world, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**1.3.2** — Passing through

| OREF | SREF |
|------|------|
| SELF-01 | ENV-PEACEFUL |

```
Medium shot, elongated figure passes through mirror surface, body stretched and distorted by liquid glass transition, half in cold corridor half in warm organic world, mirror wrapping around form like membrane, crossing between worlds, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**1.3.3** — Emerging into bone world

| OREF | SREF |
|------|------|
| SELF-01 | ENV-PEACEFUL |

```
Wide shot, elongated figure stumbles through into vast organic cathedral space, emerging from mirror that hangs in void behind, first steps into flesh architecture world, membrane arches tower above, tissue columns rise in distance, ochre sepia warmth surrounds, Zdzislaw Beksinski style, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**1.3.4** — Last look back

| OREF | SREF |
|------|------|
| SELF-01 | ENV-PEACEFUL |

```
Over-shoulder shot from behind figure in profile, looking back at mirror doorway showing cold corridor beyond, face lit by warm ochre from organic world ahead, leaving reality behind, point of no return, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

# ACT 2: SEDUCTION (0:45 - 1:10)
*10 images — Wonder, beauty, the trap forming*

---

## Scene 2.1: First Wonder (0:45 - 0:55) — 5 images

**2.1.1** — POV: First view of bone world

| OREF | SREF |
|------|------|
| — | ENV-PEACEFUL |

```
POV first-person perspective seeing organic world for first time, gentle cathedral arches of stretched membrane rise in soft ochre light, tissue towers in serene distance, beautiful organic architecture inviting exploration, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture, no figure visible --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**2.1.2** — Wonder on face

| OREF | SREF |
|------|------|
| SELF-01 | ENV-PEACEFUL |

```
Close-up elongated face looking around with wonder, expression of awe at alien beauty, pale features warmly lit by ochre ambient light, wide eyes taking in impossible architecture, first moments of enchantment, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 1:1 --v 7 --s 400
```

---

**2.1.3** — Exploring the cathedral

| OREF | SREF |
|------|------|
| SELF-01 | ENV-PEACEFUL |

```
Medium tracking shot, elongated figure walks through vast organic cathedral space, reaching up to touch membrane arch overhead, dwarfed by flesh architecture, ochre light filtering through tissue structures, gentle exploration, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**2.1.4** — Touching bone architecture

| OREF | SREF |
|------|------|
| SELF-01 | ENV-PEACEFUL |

```
Close shot, pale elongated hand touching surface of organic wall, texture like stretched membrane and sinew, organic warmth beneath fingertips, intimate contact with environment, flesh meeting flesh architecture, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**2.1.5** — Figure small in vastness

| OREF | SREF |
|------|------|
| SELF-01 | ENV-PEACEFUL |

```
Extreme wide shot, elongated figure stands tiny in center of enormous organic cathedral chamber, membrane arches soar overhead, tissue columns surround, scale emphasizes vulnerability, peaceful immensity, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

## Scene 2.2: The Trap Forms (0:55 - 1:10) — 5 images

**2.2.1** — Environment responds to presence

| OREF | SREF |
|------|------|
| SELF-01 | ENV-PEACEFUL |

```
Medium wide shot, organic architecture subtly shifts around elongated figure, flesh structures seeming to orient toward the visitor, gentle movement in peripheral vision, the environment becoming aware, watching beginning, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**2.2.2** — Beauty deepens

| OREF | SREF |
|------|------|
| SELF-01 | ENV-PEACEFUL |

```
Medium shot, elongated figure reaches toward beautiful organic formation, flesh shape like frozen music, seductive architecture inviting touch, deeper enchantment, the trap beautiful, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**2.2.3** — Mirror doorway now distant

| OREF | SREF |
|------|------|
| SELF-01 | ENV-PEACEFUL |

```
Wide shot, elongated figure in profile has wandered deep into organic world, mirror doorway now tiny and distant behind, surrounded by flesh architecture, path back unclear, gentle trap closing, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**2.2.4** — Environment closes around

| OREF | SREF |
|------|------|
| SELF-01 | ENV-PEACEFUL |

```
Medium shot, organic structures have shifted closer around elongated figure, flesh walls now nearer, space tightening subtly, beautiful prison forming, figure doesn't notice yet, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**2.2.5** — Trapped in beauty

| OREF | SREF |
|------|------|
| SELF-01 | ENV-PEACEFUL |

```
Wide establishing shot, elongated figure now completely surrounded by organic architecture, no clear exit visible, beautiful flesh prison complete, mirror doorway lost, gentle horror of realization coming, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

# ACT 3: TRANSFORMATION (1:10 - 2:30)
*45 images — Alternating slow verses and violent choruses*

---

## Scene 3.1: First Changes — VERSE (1:10 - 1:25) — 6 images

**3.1.1** — Something feels wrong

| OREF | SREF |
|------|------|
| SELF-01 | ENV-PEACEFUL |

```
Medium shot, elongated figure pauses, expression shifting to unease, something feels wrong but cannot identify what, hand touching own arm uncertainly, first stirring of dread, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**3.1.2** — Examining hand — first sign

| OREF | SREF |
|------|------|
| SELF-02 | ENV-PEACEFUL |

```
Extreme close-up of elongated hand, edges beginning to blur and soften, fingertips becoming slightly translucent, first visible sign of dissolution, subtle wrongness in familiar flesh, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/dcf1f9be-66e4-47a1-b223-68f724d3a9ea?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**3.1.3** — Confusion and denial

| OREF | SREF |
|------|------|
| SELF-02 | ENV-PEACEFUL |

```
Medium shot, elongated figure examines own arms and body, expression of confusion, edges visibly blurring now, early dissolution showing, trying to understand what is happening, denial mixing with dawning fear, Zdzislaw Beksinski style, ochre sepia palette, dreamlike horror, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/dcf1f9be-66e4-47a1-b223-68f724d3a9ea?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**3.1.4** — Environment watches

| OREF | SREF |
|------|------|
| SELF-02 | ENV-PEACEFUL |

```
Wide shot, organic flesh architecture has shifted again, membrane structures clearly oriented toward figure, watching the change begin, environment aware and interested, hollow cavities in walls watching, figure small and dissolving in center, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/dcf1f9be-66e4-47a1-b223-68f724d3a9ea?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**3.1.5** — Dissolution visible

| OREF | SREF |
|------|------|
| SELF-02 | ENV-PEACEFUL |

```
Medium close shot, elongated figure's face and arms showing clear early dissolution, edges softening and blurring, translucency spreading from extremities, features losing sharp definition, slow dissolution progressing, Zdzislaw Beksinski style, ochre sepia palette, dreamlike horror, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/dcf1f9be-66e4-47a1-b223-68f724d3a9ea?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**3.1.6** — Searching for escape

| OREF | SREF |
|------|------|
| SELF-02 | ENV-PEACEFUL |

```
Medium tracking shot, dissolving elongated figure stumbles through organic flesh architecture searching for way out, edges blurring and fading, desperate exploration, organic walls shift blocking paths, no escape visible, Zdzislaw Beksinski style, ochre sepia palette, dreamlike horror, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/dcf1f9be-66e4-47a1-b223-68f724d3a9ea?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

## Scene 3.2: First Acceleration — CHORUS (1:25 - 1:40) — 10 images

**3.2.1** — Violent dissolution surge

| OREF | SREF |
|------|------|
| SELF-03 | ENV-AGGRESSIVE |

```
Medium shot INTENSE, transformation suddenly accelerates, form dissolving and unraveling rapidly, elongated figure arching in pain, violent dissolution surge, body horror intensifying, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/537bbea7-19a1-4e6e-8bfc-f52d487f4dcb?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.2.2** — Form unraveling

| OREF | SREF |
|------|------|
| SELF-03 | ENV-AGGRESSIVE |

```
Extreme close-up torso, form unraveling into fibrous threads, flesh splitting and dissolving, becoming translucent with environment visible through gaps, violent dissolution, detailed body horror, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/537bbea7-19a1-4e6e-8bfc-f52d487f4dcb?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.2.3** — Environment responds aggressively

| OREF | SREF |
|------|------|
| SELF-03 | ENV-AGGRESSIVE |

```
Wide shot, organic architecture in aggressive motion around transforming figure, flesh structures thrusting and reaching, environment excited by consumption, violent tissue landscape, figure writhing in center, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/537bbea7-19a1-4e6e-8bfc-f52d487f4dcb?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 550
```

---

**3.2.4** — Form dissolving

| OREF | SREF |
|------|------|
| SELF-03 | ENV-AGGRESSIVE |

```
Close-up face, features dissolving and becoming translucent, one eye fading, other becoming hollow, form unraveling from fading face, identity fracturing, intimate transformation horror, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, oil painting texture --oref https://www.midjourney.com/jobs/537bbea7-19a1-4e6e-8bfc-f52d487f4dcb?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 1:1 --v 7 --s 500
```

---

**3.2.5** — Arms transforming

| OREF | SREF |
|------|------|
| SELF-03 | ENV-AGGRESSIVE |

```
Medium shot, both arms heavily transformed, flesh dissolving into translucent threads and wisps, hands fading into nothing, reaching desperately at emptiness, violent change spreading through limbs, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/537bbea7-19a1-4e6e-8bfc-f52d487f4dcb?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.2.6** — Pieces falling away

| OREF | SREF |
|------|------|
| SELF-03 | ENV-AGGRESSIVE |

```
Wide shot, threads and wisps breaking away from elongated figure, floating like smoke, body fragmenting while transforming, dissolution accelerating, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/537bbea7-19a1-4e6e-8bfc-f52d487f4dcb?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.2.7** — Environment consuming flesh

| OREF | SREF |
|------|------|
| SELF-03 | ENV-AGGRESSIVE |

```
Medium shot, fallen pieces of flesh being absorbed by organic floor, architecture consuming the shed parts, feeding on transformation debris, ground incorporating flesh into tissue structure, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/537bbea7-19a1-4e6e-8bfc-f52d487f4dcb?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.2.8** — Spine exposed

| OREF | SREF |
|------|------|
| SELF-03 | ENV-AGGRESSIVE |

```
Close shot from behind, form dissolving into threads visible through translucent back, body becoming transparent merging with environment, figure becoming architecture, intimate horror detail, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/537bbea7-19a1-4e6e-8bfc-f52d487f4dcb?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.2.9** — Figure collapsing

| OREF | SREF |
|------|------|
| SELF-03 | ENV-AGGRESSIVE |

```
Medium shot, half-dissolved figure collapsing to knees, overwhelmed by violent change, body failing mid-transformation, reaching out for support finding none, dramatic fall, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/537bbea7-19a1-4e6e-8bfc-f52d487f4dcb?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**3.2.10** — Moment of stillness

| OREF | SREF |
|------|------|
| SELF-03 | ENV-AGGRESSIVE |

```
Wide shot, half-dissolved figure frozen on knees, eye of the storm pause, aggressive environment suspended around, horrific tableau before verse slows things, calm before continuation, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/537bbea7-19a1-4e6e-8bfc-f52d487f4dcb?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

## Scene 3.3: False Hope — VERSE (1:40 - 1:55) — 6 images

**3.3.1** — Transformation pauses

| OREF | SREF |
|------|------|
| SELF-03 | ENV-PEACEFUL |

```
Medium shot, half-transformed elongated figure, transformation has slowed, moment of relief, examining own hybrid form with horror and acceptance, dissolving and solid coexist, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/537bbea7-19a1-4e6e-8bfc-f52d487f4dcb?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**3.3.2** — Examining changed body

| OREF | SREF |
|------|------|
| SELF-03 | ENV-PEACEFUL |

```
Close shot, half-solid half-translucent hand held before face, fingers partially dissolved into threads, figure studying what they're becoming, intimate moment with transformation, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/537bbea7-19a1-4e6e-8bfc-f52d487f4dcb?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**3.3.3** — Standing, searching again

| OREF | SREF |
|------|------|
| SELF-03 | ENV-PEACEFUL |

```
Medium shot, half-dissolved figure rises and begins moving again, searching for escape or cure, stubborn survival instinct, moving through watching organic architecture, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/537bbea7-19a1-4e6e-8bfc-f52d487f4dcb?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**3.3.4** — Environment blocks paths

| OREF | SREF |
|------|------|
| SELF-03 | ENV-PEACEFUL |

```
Wide shot, organic structures have shifted to block all exits, flesh walls now impassable, figure realizes escape is impossible, prison revealed, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/537bbea7-19a1-4e6e-8bfc-f52d487f4dcb?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**3.3.5** — Finds embedded mirror

| OREF | SREF |
|------|------|
| SELF-03 | ENV-PEACEFUL |

```
Medium shot, half-dissolved figure discovers mirror embedded in organic wall, hope resurging, cold silver surface in warm flesh architecture, potential escape visible, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/537bbea7-19a1-4e6e-8bfc-f52d487f4dcb?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**3.3.6** — Rushing toward mirror

| OREF | SREF |
|------|------|
| SELF-03 | ENV-PEACEFUL |

```
Medium tracking shot, half-dissolved figure rushes toward embedded mirror, desperate movement, hope driving broken body forward, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/537bbea7-19a1-4e6e-8bfc-f52d487f4dcb?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

## Scene 3.4: Second Acceleration — CHORUS (1:55 - 2:10) — 10 images

**3.4.1** — Reaching for mirror

| OREF | SREF |
|------|------|
| SELF-03 | ENV-AGGRESSIVE |

```
Medium shot, half-dissolved figure reaches toward mirror but transformation SURGES, dissolution racing up arms toward reaching hand, body betraying escape attempt, violent prevention, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/537bbea7-19a1-4e6e-8bfc-f52d487f4dcb?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.4.2** — Massive transformation surge

| OREF | SREF |
|------|------|
| SELF-04 | ENV-AGGRESSIVE |

```
Medium shot, elongated figure nearly entirely dissolved now, violent transformation surge stripped most remaining solidity, hollow silhouette emerging rapidly, only traces of fading form at edges, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/c47b3f33-24a3-4366-943e-c35a9866b4c2?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.4.3** — Flesh ripping away

| OREF | SREF |
|------|------|
| SELF-03 | ENV-AGGRESSIVE |

```
Extreme close-up, last solid pieces of form tearing away into threads, flesh ripping apart into dissolving wisps, final unraveling, detailed transformation climax, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/537bbea7-19a1-4e6e-8bfc-f52d487f4dcb?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.4.4** — Silhouette forming

| OREF | SREF |
|------|------|
| SELF-04 | ENV-AGGRESSIVE |

```
Wide shot, elongated dissolving form now dominant, recognizable hunched posture preserved as hollow silhouette, wisps of former self still trailing, environment frenzy around, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/c47b3f33-24a3-4366-943e-c35a9866b4c2?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.4.5** — Environment consuming all flesh

| OREF | SREF |
|------|------|
| SELF-04 | ENV-AGGRESSIVE |

```
Wide shot, organic architecture aggressively absorbing all shed flesh pieces, walls growing with incorporated material, feeding complete, dissolving figure in center of consumption frenzy, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/c47b3f33-24a3-4366-943e-c35a9866b4c2?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 550
```

---

**3.4.6** — Last flesh trace

| OREF | SREF |
|------|------|
| SELF-04 | ENV-AGGRESSIVE |

```
Extreme close-up, last solid patch on fading translucent hand, final human trace about to dissolve away, moment before completion, intimate final detail, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, oil painting texture --oref https://www.midjourney.com/jobs/c47b3f33-24a3-4366-943e-c35a9866b4c2?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**3.4.7** — Complete dissolving figure stands

| OREF | SREF |
|------|------|
| SELF-05 | ENV-AGGRESSIVE |

```
Medium shot, transformation complete, elongated dissolving figure stands where flesh being was, hollow dissolving form with same distinctive posture, identity consumed, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.4.8** — Dissolving figure merges with environment

| OREF | SREF |
|------|------|
| SELF-05 | ENV-AGGRESSIVE |

```
Wide shot, dissolving figure now indistinguishable in color and texture from organic architecture surrounding, became what consumed them, part of the Other, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**3.4.9** — New being stands

| OREF | SREF |
|------|------|
| SELF-05 | ENV-AGGRESSIVE |

```
Wide establishing shot, hollow dissolving being stands in vast organic cathedral, architecture and figure now matching, ochre palette unified, transformation complete, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**3.4.10** — Environment settles

| OREF | SREF |
|------|------|
| SELF-05 | ENV-PEACEFUL |

```
Wide shot, aggressive environment calming after feeding frenzy, organic architecture settling into new configuration, dissolving figure standing still amid quieting flesh structures, aftermath of consumption, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

## Scene 3.5: What Remains — VERSE (2:10 - 2:20) — 5 images

**3.5.1** — Dissolving figure examines self

| OREF | SREF |
|------|------|
| SELF-05 | ENV-PEACEFUL |

```
Medium shot, hollow silhouette examines own fading hands, trying to understand what it has become, alien to itself, quiet horror of completion, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**3.5.2** — Memory in posture

| OREF | SREF |
|------|------|
| SELF-05 | ENV-PEACEFUL |

```
Medium shot, dissolving form unconsciously assumes familiar hunched posture, body memory preserved, ghost of former self in stance, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**3.5.3** — Walking through bone world

| OREF | SREF |
|------|------|
| SELF-05 | ENV-PEACEFUL |

```
Wide shot, dissolving figure walks through organic architecture, movement matching environment rhythm, becoming one with the Other, assimilation in motion, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**3.5.4** — Discovers final mirror

| OREF | SREF |
|------|------|
| SELF-05 | ENV-PEACEFUL |

```
Medium shot, dissolving figure discovers ornate mirror floating in organic void, different from embedded one, special, drawn toward it with purpose, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**3.5.5** — Approaching final mirror

| OREF | SREF |
|------|------|
| SELF-05 | ENV-PEACEFUL |

```
Medium tracking shot, dissolving figure approaches floating mirror with slow deliberate steps, anticipation building, revelation imminent, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

## Scene 3.6: Third Acceleration / The Revelation — CHORUS (2:20 - 2:30) — 8 images

**3.6.1** — Standing before mirror

| OREF | SREF |
|------|------|
| SELF-05 | ENV-AGGRESSIVE |

```
Medium shot, dissolving figure stands directly before floating mirror, environment pulsing with energy around, moment before truth, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.6.2** — Environment shifts to watch

| OREF | SREF |
|------|------|
| SELF-05 | ENV-AGGRESSIVE |

```
Wide shot, entire organic architecture orients toward mirror and figure, environment gathering to witness revelation, massive flesh attention, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.6.3** — Looking into mirror (over shoulder)

| OREF | SREF |
|------|------|
| SELF-05 | ENV-AGGRESSIVE |

```
Over-shoulder shot, fading figure looks into mirror surface, reflection not yet revealed to viewer, body language shifts to horror, seeing something devastating, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**3.6.4** — THE TRUTH: Trapped self in mirror

| OREF | SREF |
|------|------|
| SELF-01 | ENV-AGGRESSIVE |

```
Close-up of mirror surface, reflection shows ORIGINAL FLESHED SELF trapped INSIDE the mirror, elongated humanoid with pale flesh and familiar posture pressed against glass from within, screaming silently, warm flesh imprisoned in cold reflection, the transformation revealed as EXCHANGE, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.6.5** — Both selves visible

| OREF | SREF |
|------|------|
| SELF-05 | ENV-AGGRESSIVE |

```
Wide shot showing BOTH: hollow silhouette standing OUTSIDE mirror, original fleshed self visible trapped INSIDE mirror reaching out, roles reversed, outside became inside, watcher became watched, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.6.6** — Trapped self screaming

| OREF | SREF |
|------|------|
| SELF-01 | — |

```
Close-up through mirror glass, trapped fleshed face screaming silently inside reflection, mouth open in endless despair, hands pressed against glass barrier, cannot escape, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --ar 1:1 --v 7 --s 500
```

---

**3.6.7** — Dissolving figure reaches toward mirror

| OREF | SREF |
|------|------|
| SELF-05 | ENV-AGGRESSIVE |

```
Medium shot, fading figure reaches toward mirror in horror and desperation, fading hand extending toward glass, trapped self reaching back from within, almost touching, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.6.8** — Hands almost meeting

| OREF | SREF |
|------|------|
| SELF-05 | ENV-AGGRESSIVE |

```
Extreme close-up, fading hand presses against mirror from outside, flesh hand presses from inside, same gesture opposite sides of glass, cannot connect, same person separated by transformation, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

# ACT 4: THE REALIZATION (2:30 - 3:05)
*14 images — Peak horror, desperate reaching, cost of yearning*

---

## Scene 4.1: The Prison (2:30 - 2:45) — 7 images

**4.1.1** — Trapped self pounds glass

| OREF | SREF |
|------|------|
| SELF-01 | — |

```
Medium shot from inside mirror perspective, trapped fleshed humanoid pounds fists against glass barrier, desperate to escape, warm golden-ochre lighting from within mirror prison, elongated figure confined in reflection, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --ar 16:9 --v 7 --s 450
```

---

**4.1.2** — Trapped self eyes

| OREF | SREF |
|------|------|
| SELF-01 | — |

```
Extreme close-up, fleshed eye seen through mirror glass, tears rolling down cheek, desperation in gaze, trapped soul looking out from within reflection, intimate devastating detail, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --ar 1:1 --v 7 --s 450
```

---

**4.1.3** — Dissolving figure frozen in horror

| OREF | SREF |
|------|------|
| SELF-05 | ENV-AGGRESSIVE |

```
Medium shot, hollow silhouette stands frozen before mirror, dissolving form somehow expressing horror through posture, realizing what it has become and lost, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**4.1.4** — The divide between selves

| OREF | SREF |
|------|------|
| SELF-05 | ENV-AGGRESSIVE |

```
Wide shot, fading figure and mirror with trapped self visible within, vast organic void surrounding, isolation complete, two versions of same person eternally separated, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**4.1.5** — Fading figure somehow weeping

| OREF | SREF |
|------|------|
| SELF-05 | ENV-AGGRESSIVE |

```
Close-up fading translucent face, hollow eye areas somehow expressing grief, trace of moisture on fading form perhaps last human residue, mourning lost humanity, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**4.1.6** — Trapped self pressed against glass

| OREF | SREF |
|------|------|
| SELF-01 | ENV-PEACEFUL |

```
Medium shot, trapped fleshed self pressed fully against mirror surface from within, face distorted against glass, hands spread on barrier, desperate contact attempt, warm flesh against cold glass, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**4.1.7** — Dissolving figure begins reaching desperately

| OREF | SREF |
|------|------|
| SELF-04 | ENV-AGGRESSIVE |

```
Medium shot, fading figure reaches desperately toward mirror surface, dissolving arms extending, trying to touch trapped self, desperate rescue attempt beginning, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/c47b3f33-24a3-4366-943e-c35a9866b4c2?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

## Scene 4.2: Desperate Reaching (2:45 - 3:05) — 7 images

**4.2.1** — Clawing at mirror

| OREF | SREF |
|------|------|
| SELF-05 | ENV-AGGRESSIVE |

```
Medium shot, fading figure claws at mirror surface desperately, dissolving fingers scraping against glass, trying to break through to trapped self, futile rescue attempt, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**4.2.2** — Form fragmenting from strain

| OREF | SREF |
|------|------|
| SELF-05 | ENV-AGGRESSIVE |

```
Extreme close-up, threads unraveling from fading figure's dissolving arm from strain of reaching, the attempt to reunite destroying it, form fragmenting, self-destruction through desperation, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**4.2.3** — Trapped self reaches back

| OREF | SREF |
|------|------|
| SELF-01 | — |

```
Close-up from inside mirror, trapped fleshed self reaching toward glass, toward the fading figure that was once them, matching desperation, two halves yearning for impossible reunion, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --ar 16:9 --v 7 --s 450
```

---

**4.2.4** — Figure fragmenting from effort

| OREF | SREF |
|------|------|
| SELF-05 | ENV-AGGRESSIVE |

```
Medium shot, cracks spreading through entire dissolving form from strain, body beginning to fail from effort, pieces threatening to separate, destruction accelerating, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**4.2.5** — Environment reacts to destruction

| OREF | SREF |
|------|------|
| SELF-05 | ENV-AGGRESSIVE |

```
Wide shot, organic architecture churns around dissolving figure, environment disturbed by destruction of absorbed part, flesh structures agitated, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 550
```

---

**4.2.6** — Pressing face against mirror

| OREF | SREF |
|------|------|
| SELF-05 | ENV-AGGRESSIVE |

```
Close-up, fading figure presses translucent face against mirror surface, trying to be closer to trapped self, form distorting against glass, features dissolving from pressure, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**4.2.7** — Point of shattering

| OREF | SREF |
|------|------|
| SELF-05 | ENV-AGGRESSIVE |

```
Wide shot, fading figure covered in dissolving threads, moments from total unraveling, still reaching desperately for mirror, tragic final gesture, tense stillness before dissolution, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/63b87ec3-c6da-4e61-808b-c6024f3c47ac?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

# ACT 5: SHATTERING (3:05 - 3:23)
*7 images — Fragmentation, absorption, final image*

---

## Scene 5.1: The Breaking (3:05 - 3:12) — 4 images

**5.1.1** — First unraveling

| OREF | SREF |
|------|------|
| SELF-05 | ENV-APOCALYPSE |

```
Medium shot, figure UNRAVELS starting from reaching hand, threads and wisps explode outward in beautiful destruction, body dissolving into pieces, cost of yearning for what was lost, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/f9aa1070-27f1-4915-98b9-feb99001d014?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 550
```

---

**5.1.2** — Cascade of fragments

| OREF | SREF |
|------|------|
| SELF-05 | ENV-APOCALYPSE |

```
Wide shot, dissolving body fragmenting into countless threads, wisps scatter in all directions, form dissolving completely, beautiful dissolution, Zdzislaw Beksinski style, amber ochre palette, intense atmosphere, harsh dramatic lighting, oil painting texture --oref https://www.midjourney.com/jobs/e48ee13a-79d7-48bf-b623-122ac737677e?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/f9aa1070-27f1-4915-98b9-feb99001d014?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**5.1.3** — Trapped self watches destruction

| OREF | SREF |
|------|------|
| SELF-01 | — |

```
Close-up from inside mirror, trapped fleshed face watches figure unravel outside glass, expression of grief and horror, witnessing own death from within prison, tears streaming, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --ar 1:1 --v 7 --s 450
```

---

**5.1.4** — Threads and wisps floating

| OREF | SREF |
|------|------|
| — | ENV-APOCALYPSE |

```
Wide shot, countless dissolving threads floating through vast void, what was once a being now scattered geometry, peaceful dissolution, fragments drift slowly, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture, no figure --sref https://www.midjourney.com/jobs/f9aa1070-27f1-4915-98b9-feb99001d014?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

## Scene 5.2: Into the Void (3:12 - 3:23) — 3 images

**5.2.1** — Environment absorbs fragments

| OREF | SREF |
|------|------|
| — | ENV-APOCALYPSE |

```
Medium shot, organic architecture absorbs floating fragments, flesh structures consuming shattered pieces, the Other reclaiming what it made, architecture growing with new material, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --sref https://www.midjourney.com/jobs/f9aa1070-27f1-4915-98b9-feb99001d014?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**5.2.2** — Mirror alone

| OREF | SREF |
|------|------|
| SELF-01 | ENV-PEACEFUL |

```
Wide shot, single ornate mirror floats alone in vast organic void, only artifact remaining, trapped fleshed self still visible inside pressing against glass, surrounding architecture pulses slowly satisfied, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**5.2.3** — FINAL IMAGE: Eternal prison

| OREF | SREF |
|------|------|
| SELF-01 | ENV-PEACEFUL |

```
Wide establishing shot, mirror floating in infinite organic cathedral void, trapped elongated humanoid self visible small within pressing against glass eternally, vast ochre flesh architecture surrounding watching breathing, the Other victorious forever, Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft pulsing amber light, oil painting texture, eternal imprisonment complete --oref https://www.midjourney.com/jobs/5918fde7-8074-46d4-91c9-52a1379804f8?index=0&folder=selfless%20v1 --ow 250 --sref https://www.midjourney.com/jobs/58b9464b-d3a9-4a0e-90c4-7cc45f0c1b1f?index=0&folder=selfless%20v1 --sw 100 --ar 16:9 --v 7 --s 450
```

---

# QUICK REFERENCE TABLES

## Character Reference by Scene

| Act/Scene | Stage | Reference |
|-----------|-------|-----------|
| ACT 1 (all) | Intact flesh | SELF-01 |
| ACT 2 (all) | Intact flesh | SELF-01 |
| 3.1 | Edges blurring | SELF-02 |
| 3.2 | Mid-dissolution | SELF-03 |
| 3.3 | Mid-dissolution | SELF-03 |
| 3.4 (early) | Transitioning | SELF-03 → SELF-04 |
| 3.4 (late) | Hollow silhouette | SELF-04 → SELF-05 |
| 3.5 | Fading remnant | SELF-05 |
| 3.6 | Fading + Trapped | SELF-05 + SELF-01 (in mirror) |
| ACT 4 | Fading + Trapped | SELF-05 + SELF-01 (in mirror) |
| ACT 5 | Fragmenting + Trapped | SELF-05 + SELF-01 (in mirror) |

## Environment Reference by Section

| Section | Intensity | Reference |
|---------|-----------|-----------|
| ACT 1 (labyrinth) | Cold liminal | ENV-MIRROR |
| ACT 2 (entry) | Peaceful | ENV-PEACEFUL |
| ACT 2 (trap) | Watching | ENV-PEACEFUL |
| Verses (slow) | Peaceful/Watching | ENV-PEACEFUL |
| Choruses (fast) | Aggressive | ENV-AGGRESSIVE |
| Climax (revelation) | Aggressive | ENV-AGGRESSIVE |
| Shattering | Apocalyptic | ENV-APOCALYPSE |
| Final image | Watching | ENV-PEACEFUL |

---

# TOTAL IMAGE COUNT: 90 images

| Act | Images | Time |
|-----|--------|------|
| ACT 1 | 14 | 0:00 - 0:45 |
| ACT 2 | 10 | 0:45 - 1:10 |
| ACT 3.1 (verse) | 6 | 1:10 - 1:25 |
| ACT 3.2 (chorus) | 10 | 1:25 - 1:40 |
| ACT 3.3 (verse) | 6 | 1:40 - 1:55 |
| ACT 3.4 (chorus) | 10 | 1:55 - 2:10 |
| ACT 3.5 (verse) | 5 | 2:10 - 2:20 |
| ACT 3.6 (chorus) | 8 | 2:20 - 2:30 |
| ACT 4 | 14 | 2:30 - 3:05 |
| ACT 5 | 7 | 3:05 - 3:23 |

---

# PRODUCTION CHECKLIST

```
STEP 1 - CREATE CHARACTER REFERENCES (5 images):
[ ] SELF-01 (intact flesh) generated and URL saved
[ ] SELF-02 (edges blurring) generated and URL saved
[ ] SELF-03 (mid-dissolution) generated and URL saved
[ ] SELF-04 (hollow silhouette) generated and URL saved
[ ] SELF-05 (fading remnant) generated and URL saved

STEP 2 - CREATE ENVIRONMENT REFERENCES (4 images):
[ ] ENV-MIRROR (cold labyrinth) generated and URL saved
[ ] ENV-PEACEFUL (peaceful bone) generated and URL saved
[ ] ENV-AGGRESSIVE (violent bone) generated and URL saved
[ ] ENV-APOCALYPSE (shattering) generated and URL saved

STEP 3 - GENERATE SCENE IMAGES (90 images):
[ ] ACT 1 Scene 1.1 (5 images)
[ ] ACT 1 Scene 1.2 (5 images)
[ ] ACT 1 Scene 1.3 (4 images)
[ ] ACT 2 Scene 2.1 (5 images)
[ ] ACT 2 Scene 2.2 (5 images)
[ ] ACT 3 Scene 3.1 VERSE (6 images)
[ ] ACT 3 Scene 3.2 CHORUS (10 images)
[ ] ACT 3 Scene 3.3 VERSE (6 images)
[ ] ACT 3 Scene 3.4 CHORUS (10 images)
[ ] ACT 3 Scene 3.5 VERSE (5 images)
[ ] ACT 3 Scene 3.6 CHORUS (8 images)
[ ] ACT 4 Scene 4.1 (7 images)
[ ] ACT 4 Scene 4.2 (7 images)
[ ] ACT 5 Scene 5.1 (4 images)
[ ] ACT 5 Scene 5.2 (3 images)

STEP 4 - POST-PRODUCTION:
[ ] Import all 90 images to video editor
[ ] Arrange in sequence order
[ ] Sync to music beats
[ ] Add Ken Burns pan/zoom effects
[ ] Add transitions (dissolves for verses, hard cuts for choruses)
[ ] Color grade for consistency
[ ] Export final video
```

---

# STYLE CONSISTENCY NOTES

## Beksiński Style Checklist

Every generated image should have:
- [ ] Ochre/sepia/amber/umber color palette
- [ ] Soft diffuse lighting (no harsh shadows except in chorus scenes)
- [ ] Oil painting texture feel
- [ ] Dreamlike atmospheric haze at edges
- [ ] Organic bone/flesh architecture (not geometric crystal)
- [ ] Elongated figure proportions maintained
- [ ] Melancholic mood even in horror

## Common Prompt Suffixes

**For verses (peaceful/slow):**
```
Zdzislaw Beksinski style, ochre sepia palette, dreamlike atmosphere, soft diffuse lighting, oil painting texture --ar 16:9 --v 7 --s 400-450
```

**For choruses (aggressive/fast):**
```
Zdzislaw Beksinski style, amber umber palette, intense atmosphere, harsh dramatic lighting, oil painting texture --ar 16:9 --v 7 --s 500-550
```

**For portraits/close-ups:**
```
Zdzislaw Beksinski style, ochre tones, intimate portrait, soft focus edges --ar 1:1 --v 7 --s 450
```

---

# LYRICS-TO-SCENE SYNC

Use this for timing specific images to lyrics in Vegas Pro.

| Lyric | Suggested Scene(s) | Image # | Notes |
|-------|-------------------|---------|-------|
| **"I beg you, take me"** | 1.2.4 — The inviting mirror | #9 | Figure reaching toward glowing mirror portal |
| **"With you"** | 1.3.2 — Passing through | #12 | Body crossing through mirror surface |
| **"I give you meaning"** | 2.1.4 — Touching bone architecture | #19 | Intimate contact with environment |
| **"You owe me life"** | 2.2.1 — Environment responds | #21 | Environment becoming aware, mutual exchange begins |
| **"All for this fight"** | 3.2.1 — Violent dissolution surge | #31 | First chorus acceleration |
| **"Lost for myself"** | 3.2.4 — Form dissolving | #34 | Identity fracturing visually |
| **"Such a likely story"** | 3.3.1 — Transformation pauses | #41 | Ironic calm, examining changed body |
| **"Here I am"** | 3.3.4 — Environment blocks paths | #44 | Trapped, no escape, accepting fate |
| **"I'll live it all for"** | 3.4.4 — Silhouette forming | #52 | Becoming what consumed them |
| **"Pleasing just you"** | 3.4.5 — Environment consuming all flesh | #53 | Feeding complete, environment satisfied |
| **"Self-appointed slavery"** | 3.4.7 — Complete dissolving figure stands | #55 | Transformation complete by choice |
| **"I need to survive"** | 3.5.4 — Discovers final mirror | #63 | Last hope, false survival instinct |
| **"Take me with you"** (reprise) | 3.6.4 — THE TRUTH revealed | #68 | Devastating reveal of trapped self |
| **"You owe me your life"** | 4.1.5 — Fading figure weeping | #75 | Role reversal — dissolving figure mourns |
| **"All for my fight"** | 4.2.4 — Figure fragmenting | #82 | Self-destruction through reaching |
| **"Lost for yourself"** | 5.1.3 — Trapped self watches destruction | #87 | Witnessing own death from within prison |
| **"You depend on this"** | 5.2.1 — Environment absorbs fragments | #88 | Environment consuming, completing cycle |
| **"Yourself-lessness"** | 5.2.3 — FINAL IMAGE | #90 | Eternal imprisonment, SELF-LESS forever |

## Timing Strategy

**Verses (slower):**
- Hold images longer (2.5-3.5 seconds)
- Dissolve transitions
- Match contemplative moments

**Choruses (faster):**
- Quick cuts (1-2 seconds)
- Hard cuts or flash transitions
- Match intense lyrics to transformation violence

**Key Sync Points:**
- "Lost for myself" → Form dissolving (exact hit)
- "Self-appointed slavery" → Complete dissolution (revelation)
- Final "yourself-lessness" → Hold on final image through end

---

# THE MESSAGE

**"Selfless" = Becoming SELF-LESS**

When you give yourself completely to another, you don't just lose yourself — you become the thing that consumed you, and your true self becomes a prisoner you can never reach again.

The environment won. It always wins. It always has.
