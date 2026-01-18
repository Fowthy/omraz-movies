# SELFLESS — Music Video Production Guide
## Midjourney V7 Complete Edition with Character Consistency

---

# THE STORY

**"Selfless" = Becoming SELF-LESS (empty, no identity)**

THE SELF is a humanoid being searching for their reflection in an infinite mirror labyrinth. But every mirror shows something wrong — not their face, but glimpses of a red crystalline void. THE OTHER is not a character but the environment itself: a living, breathing red crystalline dimension that watches, waits, and hungers.

Drawn by obsession, THE SELF steps through a mirror and enters this crimson geometric world. At first it's peaceful, beautiful, seductive. But the environment begins to consume them. Their flesh cracks. Crystals grow from their skin. With each verse, the change creeps slowly. With each chorus, it accelerates violently.

THE SELF explores deeper, hoping to find themselves, but only loses more. The red crystalline environment shifts and morphs constantly — it IS the Other, surrounding them completely, absorbing them piece by piece.

In the climax, THE SELF finds one final mirror. They look in and see the horror: they have BECOME part of the red crystalline environment. Their old human self is trapped IN the mirror, looking back, screaming silently. The watcher has become the watched. The consumed has become the consumer.

Desperate, the now-crystalline being reaches for the mirror, trying to touch their old self. But the strain shatters them. They fragment into a thousand red crystalline shards, scattering into the void. The environment — THE OTHER — absorbs these pieces.

Final image: the mirror floats alone in the red crystalline void. Inside it, the trapped human SELF presses against the glass forever. The environment pulses. It has won. It has always won.

**The message:** When you give yourself completely to another, you don't just lose yourself — you become the thing that consumed you, and your true self becomes a prisoner you can never reach again.

---

# REFERENCE SYSTEM EXPLAINED

## How Consistency Works in Midjourney V7

| Parameter | What It Does | Weight Control |
|-----------|--------------|----------------|
| `--oref [URL]` | Keeps character/object consistent | `--ow 200` (your choice) |
| `--sref [URL]` | Keeps visual style/aesthetic consistent | `--sw 100` (default) |

**You can combine both:** `prompt text --oref [char URL] --ow 200 --sref [style URL] --sw 100`

## Reference Image Strategy

**THE SELF (Character):** Hybrid approach
- **ACT 1-2:** Use `SELF-01` (intact human)
- **ACT 3:** Transition through `SELF-02` → `SELF-03` → `SELF-04`
- **ACT 4-5:** Use `SELF-04` (crystalline) + `SELF-01` (trapped in mirror)

**THE OTHER (Environment Style):** Match intensity to scene
- **Verses:** Use `OTHER-01` (peaceful) or `OTHER-02` (active)
- **Choruses:** Use `OTHER-03` (aggressive)
- **Ending:** Use `OTHER-04` (apocalyptic)

---

# STEP 1: CREATE REFERENCE IMAGES FIRST

Generate these 8 images and save them. You'll use their URLs for all subsequent generations.

## THE SELF — Character References

### SELF-01: Intact/Beginning (Use for ACT 1-2)
```
Ethereal humanoid figure with luminous porcelain skin, delicate androgynous features, subtle golden veins visible beneath translucent flesh, warm amber light emanating from chest cavity, wearing tattered flowing white fabric, expression of searching and longing, whole and beautiful and vulnerable, full body standing pose facing camera, pure black void background, clear front-facing view for reference, experimental anime aesthetic, soft volumetric lighting --ar 16:9 --v 7 --s 350
```
> **IMPORTANT:** Choose the clearest front-facing result. This is your main character reference.

### SELF-02: Early Deterioration (Use for ACT 3 early)
```
Same ethereal humanoid figure with hairline fractures spreading across pale porcelain skin, small red crystalline growths emerging at fingertips and along spine, expression of confusion and dawning fear, warm flesh tones beginning to shift cooler at extremities, golden inner light dimming slightly, same tattered white garments, full body standing pose facing camera, black void background, clear reference view, detailed body horror aesthetic --ar 16:9 --v 7 --s 350
```

### SELF-03: Mid-Transformation (Use for ACT 3 middle)
```
Same humanoid figure now half flesh half red crystal, face splitting between organic features and geometric crimson facets, one eye human with tears one eye ruby crystal, skin peeling away revealing blood-red crystalline structure beneath, body showing significant transformation, warm golden tones invaded by deep crimson, full body pose facing camera, black void background, clear reference view, surreal body horror art --ar 16:9 --v 7 --s 400
```

### SELF-04: Near-Complete/Crystalline (Use for ACT 3 late, ACT 4-5)
```
Same figure almost entirely transformed into red crystalline being, last traces of human face visible beneath faceted ruby surface, humanoid silhouette made of geometric crimson facets, one hand still slightly flesh reaching desperately, deep crimson dominates with dying hints of original golden warmth, full body pose facing camera, pure black void background, clear reference view, beautiful horror aesthetic --ar 16:9 --v 7 --s 400
```

---

## THE OTHER — Environment Style References

### OTHER-01: Peaceful/Seductive (Use for verses, early scenes)
```
Vast serene red crystalline landscape floating in infinite void, gentle ruby formations drift slowly like frozen music, soft crimson facets glow with warm inner light, geometric shapes shift almost imperceptibly, beautiful and inviting with subtle wrongness, delicate scarlet spires form impossible archways, deep blood-red fading to soft rose at edges, the space feels alive and breathing slowly, surreal crystalline dreamscape, cinematic wide establishing shot, soft ambient lighting, no figures --ar 16:9 --v 7 --s 400
```

### OTHER-02: Active/Watching (Use for transitions, tense verses)
```
Infinite red crystalline void where the environment is alive and aware, massive ruby geometric formations shift morph and reconfigure continuously, faceted crimson surfaces seem oriented and watching, deep blood-red with black shadows between formations, crystalline spires grow and dissolve endlessly, no sky no ground only shifting red architecture, alien landscape that breathes and observes, surreal environment, wide shot, volumetric crimson light, no figures --ar 16:9 --v 7 --s 450
```

### OTHER-03: Aggressive/Consuming (Use for choruses)
```
Violent red crystalline dimension in aggressive flux, massive ruby formations thrust upward and collapse rapidly, sharp crimson geometric shapes multiply and swarm, the living environment reaches and grasps hungrily, faceted scarlet surfaces pulse with predatory energy, deep blood-red with harsh black shadows, crystalline chaos surrounds and overwhelms, geometry that devours, apocalyptic surreal horror landscape, dynamic wide shot, harsh dramatic red lighting, no figures --ar 16:9 --v 7 --s 500
```

### OTHER-04: Apocalyptic/Shattering (Use for ending)
```
Cataclysmic red crystalline void in violent collapse, massive ruby formations shatter and explode into infinite fragments, crimson geometric reality tears itself apart in death throes, scarlet shards rain in all directions defying physics, black fissures split through dying red surfaces like wounds, the watching geometry now screaming and dying, total annihilation of crystalline space, deep crimson fading to void black, apocalyptic surreal destruction, extreme wide shot, chaotic harsh lighting, no figures --ar 16:9 --v 7 --s 550
```

---

# REFERENCE ASSIGNMENT LEGEND

For each image prompt below, the reference box shows:
- **OREF:** Which character image URL to use with `--oref`
- **SREF:** Which style image URL to use with `--sref`
- **Full suffix:** The complete parameter string to add

**Example format:**
```
[Your prompt text] --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --sref https://www.midjourney.com/jobs/104deaa1-7824-4248-8aad-62a240b8130c?index=2 --sw 100 --ar 16:9 --v 7
```

---

# ACT 1: THE MIRROR LABYRINTH (0:00 - 0:45)
*Verses — Beautiful, slow dread*

## Scene 1.1: Discovery (0:00 - 0:15) — 4 images

---

**1.1.1** — Wide establishing

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | — (mirror environment, not red void yet) |

```
Infinite corridor of mirrors stretching in all directions, impossible geometry Escher-like architecture, liminal backrooms quality, cold silver-blue reflective surfaces, pale humanoid figure stands small in center searching, warm golden glow from figure contrasts cold environment, endless reflections multiply into darkness, surreal mirror labyrinth, cinematic wide establishing shot, volumetric fog, eerie stillness --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --ar 16:9 --v 7 --s 350
```

---

**1.1.2** — Figure searching

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | — |

```
Ethereal humanoid figure with porcelain skin walks through infinite mirror corridor, golden light emanating from chest, expression of longing and searching, looking into each mirror passed, tattered flowing garments drift, warm figure in cold reflective environment, experimental anime aesthetic, medium tracking shot, soft volumetric lighting --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --ar 16:9 --v 7 --s 350
```

---

**1.1.3** — Wrong reflection reveal

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | OTHER-01 |

```
Humanoid figure stands before ornate mirror, but reflection shows red crystalline void instead of face, crimson geometric shapes where features should be, figure hasn't noticed the wrongness yet, warm flesh meets cold glass meets impossible crimson reflection, surreal horror moment, medium shot over shoulder into mirror, dramatic lighting contrast --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --sref https://www.midjourney.com/jobs/104deaa1-7824-4248-8aad-62a240b8130c?index=2 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**1.1.4** — Multiple wrong mirrors

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | OTHER-01 |

```
Wide shot mirror corridor, pale humanoid figure walks between mirrors, every reflection shows glimpses of red crystalline geometry instead of the figure, crimson facets visible in silver frames, figure continues unaware, surrounded by wrongness, liminal horror atmosphere, tracking wide shot, cold blue environment warm golden figure --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --sref https://www.midjourney.com/jobs/104deaa1-7824-4248-8aad-62a240b8130c?index=2 --sw 100 --ar 16:9 --v 7 --s 350
```

---

## Scene 1.2: The Watcher Revealed (0:15 - 0:30) — 4 images

---

**1.2.1** — Red in the mirrors

| Reference | Image |
|-----------|-------|
| OREF | — (no character in frame) |
| SREF | OTHER-01 |

```
Close-up of ornate mirror frame, reflection filled entirely with shifting red crystalline geometry, ruby facets pulse with inner light, sense of something vast watching through the glass, crimson void behind the surface, no human reflection at all, beautiful and wrong, extreme close-up mirror surface, soft glow from within --sref https://www.midjourney.com/jobs/104deaa1-7824-4248-8aad-62a240b8130c?index=2 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**1.2.2** — Figure notices

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | OTHER-01 |

```
Humanoid figure stops before mirror, expression shifting to confusion, hand raised toward reflection that shows red crystalline void instead of hand, first moment of awareness something is wrong, warm golden figure against cold silver mirror containing crimson geometry, medium shot, dramatic rim lighting --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --sref https://www.midjourney.com/jobs/104deaa1-7824-4248-8aad-62a240b8130c?index=2 --sw 100 --ar 16:9 --v 7 --s 350
```

---

**1.2.3** — Surrounded

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | OTHER-02 |

```
Wide overhead shot, pale humanoid figure stands at center of circular mirror chamber, every mirror surface filled with red crystalline void watching, figure small and alone surrounded by crimson geometric reflections, trapped in observation, beautiful horror composition, crane shot looking down, volumetric light --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --sref https://www.midjourney.com/jobs/2d500449-a6a6-4853-ad4e-1d5470f49845?index=1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**1.2.4** — The invitation

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | OTHER-01 |

```
Single mirror glows with soft warm red light, inviting rather than threatening, beautiful crimson crystalline vista visible through the glass like a doorway, peaceful ruby landscape beckoning, figure drawn toward it hand reaching, seductive trap revealed, medium shot figure approaching glowing mirror, warm red light on face --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --sref https://www.midjourney.com/jobs/104deaa1-7824-4248-8aad-62a240b8130c?index=2 --sw 100 --ar 16:9 --v 7 --s 350
```

---

## Scene 1.3: Drawn Closer (0:30 - 0:45) — 4 images

---

**1.3.1** — Approaching the threshold

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | OTHER-01 |

```
Humanoid figure walks toward largest mirror, red crystalline landscape visible through glass like window to another world, peaceful ruby geometry inviting exploration, figure's golden chest light reflects off mirror surface, approaching point of no return, cinematic medium shot, building tension, warm meeting cold meeting red --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --sref https://www.midjourney.com/jobs/104deaa1-7824-4248-8aad-62a240b8130c?index=2 --sw 100 --ar 16:9 --v 7 --s 350
```

---

**1.3.2** — Hand on glass

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | OTHER-01 |

```
Extreme close-up, pale luminous hand presses against mirror surface, glass ripples like water at touch, red crystalline void visible through distorting surface, moment before crossing, flesh meeting barrier to other world, intimate detail shot, soft focus background sharp focus on hand and rippling glass --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --sref https://www.midjourney.com/jobs/104deaa1-7824-4248-8aad-62a240b8130c?index=2 --sw 100 --ar 16:9 --v 7 --s 300
```

---

**1.3.3** — Mirror yields

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | OTHER-01 |

```
Medium shot, humanoid figure's hand sinks INTO mirror surface, glass wraps around wrist like liquid silver, arm entering red crystalline dimension beyond, expression of wonder mixed with fear, crossing the threshold beginning, surreal body horror moment, dramatic side lighting --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --sref https://www.midjourney.com/jobs/104deaa1-7824-4248-8aad-62a240b8130c?index=2 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**1.3.4** — Last look back

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | OTHER-01 |

```
Over-shoulder shot from behind figure half-through mirror, looking back at normal mirror corridor one last time, face illuminated by red light from world ahead, leaving reality behind, point of no return, liminal transition moment, cinematic composition, warm figure cold corridor red destination --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --sref https://www.midjourney.com/jobs/104deaa1-7824-4248-8aad-62a240b8130c?index=2 --sw 100 --ar 16:9 --v 7 --s 350
```

---

# ACT 2: STEPPING THROUGH (0:45 - 1:00)
*Transition — Building tension*

## Scene 2.1: The Crossing (0:45 - 0:55) — 5 images

---

**2.1.1** — Through the mirror

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | OTHER-01 |

```
Humanoid figure passes through mirror surface, body stretched and distorted by liquid glass transition, half in normal space half in red crystalline void, mirror wrapping around form like membrane, surreal crossing between worlds, beautiful body distortion, medium shot, dramatic contrast between blue-silver and crimson worlds --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --sref https://www.midjourney.com/jobs/104deaa1-7824-4248-8aad-62a240b8130c?index=2 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**2.1.2** — Emergence

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | OTHER-01 |

```
Figure stumbles through into red crystalline dimension, emerging from mirror surface that hangs in void behind them, first steps into new world, vast ruby geometric landscape stretches infinitely, disoriented pose, warm figure entering crimson environment, wide shot showing scale of new world, volumetric red light --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --sref https://www.midjourney.com/jobs/104deaa1-7824-4248-8aad-62a240b8130c?index=2 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**2.1.3** — First view (POV)

| Reference | Image |
|-----------|-------|
| OREF | — (POV shot, no character visible) |
| SREF | OTHER-01 |

```
POV first-person perspective seeing red crystalline world for first time, gentle ruby formations floating peacefully, soft crimson light, beautiful and inviting vista, geometric shapes drift slowly, serene alien landscape, immersive wide angle, warm soft lighting --sref https://www.midjourney.com/jobs/104deaa1-7824-4248-8aad-62a240b8130c?index=2 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**2.1.4** — Wonder

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | OTHER-01 |

```
Medium shot, humanoid figure stands in red crystalline void looking around with wonder, expression of awe at alien beauty, soft ruby light illuminates porcelain skin, golden chest glow reflects off nearby crimson facets, peaceful moment before horror, experimental anime aesthetic, soft volumetric lighting --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --sref https://www.midjourney.com/jobs/104deaa1-7824-4248-8aad-62a240b8130c?index=2 --sw 100 --ar 16:9 --v 7 --s 350
```

---

**2.1.5** — The mirror behind

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | OTHER-01 |

```
Wide shot, figure small in vast red crystalline landscape, single mirror floating behind them showing normal world beyond, doorway still open, ruby geometric formations surround peacefully, establishing new environment, cinematic composition, contrasting worlds visible --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --sref https://www.midjourney.com/jobs/104deaa1-7824-4248-8aad-62a240b8130c?index=2 --sw 100 --ar 16:9 --v 7 --s 400
```

---

## Scene 2.2: Seduction (0:55 - 1:00) — 3 images

---

**2.2.1** — Exploring

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | OTHER-01 |

```
Humanoid figure walks through peaceful red crystalline environment, touching floating ruby formations with curiosity, soft crimson glow responds to touch, gentle interaction with alien world, beautiful and serene, figure trusting the environment, medium tracking shot, warm soft red lighting --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --sref https://www.midjourney.com/jobs/104deaa1-7824-4248-8aad-62a240b8130c?index=2 --sw 100 --ar 16:9 --v 7 --s 350
```

---

**2.2.2** — Environment responds

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | OTHER-02 |

```
Red crystalline formations shift and morph gently around humanoid figure, ruby geometry forming beautiful patterns, welcoming display, the environment actively engaging with visitor, seductive alien beauty, figure enchanted, wide shot showing surrounding movement, soft pulsing crimson light --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --sref https://www.midjourney.com/jobs/2d500449-a6a6-4853-ad4e-1d5470f49845?index=1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**2.2.3** — The trap closes

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | OTHER-02 |

```
Wide establishing shot, humanoid figure now deep within red crystalline void, mirror doorway tiny and distant behind, surrounded completely by ruby geometry, beautiful prison forming, figure doesn't realize the trap yet, vast crimson landscape, cinematic wide shot, ominous beauty --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --sref https://www.midjourney.com/jobs/2d500449-a6a6-4853-ad4e-1d5470f49845?index=1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

# ACT 3: TRANSFORMATION (1:00 - 2:30)
*Alternating Verses (slow) and Choruses (fast)*

## Scene 3.1: First Changes — VERSE (1:00 - 1:20) — 5 images

---

**3.1.1** — Subtle wrongness

| Reference | Image |
|-----------|-------|
| OREF | SELF-02 |
| SREF | OTHER-01 |

```
Medium shot, humanoid figure examining their hand, tiny hairline crack visible on knuckle, first sign of change barely noticeable, confusion on face, red crystalline environment peaceful in background, the transformation begins invisibly, intimate character moment, soft red ambient lighting --oref https://www.midjourney.com/jobs/f635f459-9a5c-452e-894f-28b1201814eb?index=0 --ow 200 --sref https://www.midjourney.com/jobs/104deaa1-7824-4248-8aad-62a240b8130c?index=2 --sw 100 --ar 16:9 --v 7 --s 350
```

---

**3.1.2** — Cracks spreading

| Reference | Image |
|-----------|-------|
| OREF | SELF-02 |
| SREF | OTHER-01 |

```
Close-up forearm and hand, more cracks visible spreading like frost on glass, small red crystalline facet emerging at fingertip, figure touching the change with other hand, dawning horror, warm flesh becoming cold crystal, detailed body horror beginning, extreme close-up, dramatic lighting --oref https://www.midjourney.com/jobs/f635f459-9a5c-452e-894f-28b1201814eb?index=0 --ow 200 --sref https://www.midjourney.com/jobs/104deaa1-7824-4248-8aad-62a240b8130c?index=2 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**3.1.3** — Environment watching

| Reference | Image |
|-----------|-------|
| OREF | SELF-02 |
| SREF | OTHER-02 |

```
Wide shot, red crystalline formations have shifted subtly, seem oriented toward humanoid figure, geometry watching without eyes, figure small and vulnerable in center, the environment is aware and interested, vast ruby landscape, sense of being observed, cinematic wide shot, volumetric crimson light --oref https://www.midjourney.com/jobs/f635f459-9a5c-452e-894f-28b1201814eb?index=0 --ow 200 --sref https://www.midjourney.com/jobs/2d500449-a6a6-4853-ad4e-1d5470f49845?index=1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**3.1.4** — Searching for help

| Reference | Image |
|-----------|-------|
| OREF | SELF-02 |
| SREF | OTHER-01 |

```
Medium shot, figure looking around desperately, more cracks visible on neck and shoulder, searching for escape or cure, red crystalline environment offers no comfort, isolation in alien beauty, expression of growing fear, experimental anime aesthetic, cold red lighting on warm flesh --oref https://www.midjourney.com/jobs/f635f459-9a5c-452e-894f-28b1201814eb?index=0 --ow 200 --sref https://www.midjourney.com/jobs/104deaa1-7824-4248-8aad-62a240b8130c?index=2 --sw 100 --ar 16:9 --v 7 --s 350
```

---

**3.1.5** — The change continues

| Reference | Image |
|-----------|-------|
| OREF | SELF-02 |
| SREF | OTHER-02 |

```
Medium shot, humanoid figure standing still as change spreads, red crystalline growths now visible along spine through torn garment, accepting what cannot be stopped, resigned horror, ruby facets catch light, warm figure being consumed by cold crystal, Beksinski surrealism, dramatic rim lighting --oref https://www.midjourney.com/jobs/f635f459-9a5c-452e-894f-28b1201814eb?index=0 --ow 200 --sref https://www.midjourney.com/jobs/2d500449-a6a6-4853-ad4e-1d5470f49845?index=1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

## Scene 3.2: First Acceleration — CHORUS (1:20 - 1:35) — 8 images

---

**3.2.1** — Violent eruption

| Reference | Image |
|-----------|-------|
| OREF | SELF-03 |
| SREF | OTHER-03 |

```
Medium shot CHAOS, red crystalline growths ERUPT from humanoid figure's back and shoulders, violent rapid transformation, body arches in agony, ruby shards burst through flesh, the change accelerates horrifically, body horror at maximum, dynamic pose, harsh dramatic crimson lighting, motion blur --oref https://www.midjourney.com/jobs/c93195a9-80f5-4314-b2fd-0f1515ea6d63?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.2.2** — Skin crystallizing

| Reference | Image |
|-----------|-------|
| OREF | SELF-03 |
| SREF | OTHER-03 |

```
Extreme close-up, flesh transforms to red faceted crystal in spreading wave, skin texture becoming geometric, organic to mineral transition visible, horrific beautiful detail, body horror transformation, macro detail shot, harsh lighting showing texture change --oref https://www.midjourney.com/jobs/c93195a9-80f5-4314-b2fd-0f1515ea6d63?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.2.3** — Environment responds

| Reference | Image |
|-----------|-------|
| OREF | SELF-03 |
| SREF | OTHER-03 |

```
Wide shot, red crystalline environment shifts aggressively, massive ruby formations thrust and multiply, responding to figure's transformation, geometry excited by consumption, violent alien landscape, figure writhes in center, chaotic dynamic composition, harsh pulsing crimson light --oref https://www.midjourney.com/jobs/c93195a9-80f5-4314-b2fd-0f1515ea6d63?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 550
```

---

**3.2.4** — Face splitting

| Reference | Image |
|-----------|-------|
| OREF | SELF-03 |
| SREF | OTHER-03 |

```
Close-up face, features splitting between flesh and red crystal, one eye human with tear one eye faceted ruby, mouth open in silent scream showing crystalline teeth, identity fracturing, intimate body horror, extreme close-up, harsh contrast lighting --oref https://www.midjourney.com/jobs/c93195a9-80f5-4314-b2fd-0f1515ea6d63?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.2.5** — Arms transforming

| Reference | Image |
|-----------|-------|
| OREF | SELF-03 |
| SREF | OTHER-03 |

```
Medium shot, both arms now heavily crystallized, red geometric growths overtaking flesh, hands becoming angular and faceted, reaching desperately at nothing, beautiful horrible transformation, body horror art, dynamic angle, volumetric red light --oref https://www.midjourney.com/jobs/c93195a9-80f5-4314-b2fd-0f1515ea6d63?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.2.6** — Fragmentation begins

| Reference | Image |
|-----------|-------|
| OREF | SELF-03 |
| SREF | OTHER-03 |

```
Wide shot, pieces of humanoid figure beginning to break away as floating crystalline shards, body fragmenting while transforming, red geometric pieces orbit the form, dissolution and consumption, surreal body horror, chaotic composition, harsh dramatic lighting --oref https://www.midjourney.com/jobs/c93195a9-80f5-4314-b2fd-0f1515ea6d63?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 550
```

---

**3.2.7** — Environment consuming

| Reference | Image |
|-----------|-------|
| OREF | SELF-03 |
| SREF | OTHER-03 |

```
Medium shot, red crystalline formations reaching toward transforming figure, ruby geometry actively taking pieces, consumption visible and aggressive, the Other feeding, alien horror landscape devouring, dynamic threatening composition, harsh crimson lighting --oref https://www.midjourney.com/jobs/c93195a9-80f5-4314-b2fd-0f1515ea6d63?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.2.8** — Moment of stillness

| Reference | Image |
|-----------|-------|
| OREF | SELF-03 |
| SREF | OTHER-03 |

```
Wide shot, figure frozen mid-transformation, half flesh half red crystal, surrounded by aggressive ruby geometry, pause in chaos, eye of the storm, horrific beautiful tableau, calm before next wave, cinematic wide shot, dramatic red lighting --oref https://www.midjourney.com/jobs/c93195a9-80f5-4314-b2fd-0f1515ea6d63?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 450
```

---

## Scene 3.3: False Hope — VERSE (1:35 - 1:50) — 4 images

---

**3.3.1** — Transformation pauses

| Reference | Image |
|-----------|-------|
| OREF | SELF-03 |
| SREF | OTHER-02 |

```
Medium shot, humanoid figure now half crystallized, red facets covering half the body, but transformation has slowed, moment of relief, examining changed form with horror and acceptance, ruby and flesh coexist, Tekkonkinkreet aesthetic, soft ambient red lighting --oref https://www.midjourney.com/jobs/c93195a9-80f5-4314-b2fd-0f1515ea6d63?index=0 --ow 200 --sref https://www.midjourney.com/jobs/2d500449-a6a6-4853-ad4e-1d5470f49845?index=1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**3.3.2** — Searching for mirror

| Reference | Image |
|-----------|-------|
| OREF | SELF-03 |
| SREF | OTHER-02 |

```
Wide shot, half-transformed figure stumbling through red crystalline void, searching for mirror doorway to escape, ruby environment peaceful again deceptively, desperate quest, vast alien landscape, figure small and determined, cinematic tracking shot, soft crimson lighting --oref https://www.midjourney.com/jobs/c93195a9-80f5-4314-b2fd-0f1515ea6d63?index=0 --ow 200 --sref https://www.midjourney.com/jobs/2d500449-a6a6-4853-ad4e-1d5470f49845?index=1 --sw 100 --ar 16:9 --v 7 --s 350
```

---

**3.3.3** — Environment shifts

| Reference | Image |
|-----------|-------|
| OREF | SELF-03 |
| SREF | OTHER-02 |

```
Medium shot, red crystalline formations have rearranged, blocking path to distant mirror, ruby geometry deliberately obstructing, figure realizes escape is prevented, the environment toys with them, vast crimson walls of crystal, trapped revelation, dramatic wide shot --oref https://www.midjourney.com/jobs/c93195a9-80f5-4314-b2fd-0f1515ea6d63?index=0 --ow 200 --sref https://www.midjourney.com/jobs/2d500449-a6a6-4853-ad4e-1d5470f49845?index=1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**3.3.4** — Finding another mirror

| Reference | Image |
|-----------|-------|
| OREF | SELF-03 |
| SREF | OTHER-02 |

```
Medium shot, half-transformed figure discovers mirror embedded in red crystalline wall, hope resurging, rushing toward it, reflection still shows their partly-human form, potential escape visible, dramatic moment, warm lighting from mirror cold red surrounding --oref https://www.midjourney.com/jobs/c93195a9-80f5-4314-b2fd-0f1515ea6d63?index=0 --ow 200 --sref https://www.midjourney.com/jobs/2d500449-a6a6-4853-ad4e-1d5470f49845?index=1 --sw 100 --ar 16:9 --v 7 --s 350
```

---

## Scene 3.4: Second Acceleration — CHORUS (1:50 - 2:05) — 8 images

---

**3.4.1** — Reaching for mirror

| Reference | Image |
|-----------|-------|
| OREF | SELF-03 |
| SREF | OTHER-03 |

```
Medium shot, half-crystallized figure reaches toward embedded mirror, but red crystal ERUPTS up arm toward hand, transformation surging to prevent escape, body horror intensifying, desperate reaching, dramatic reaching pose, harsh crimson lighting --oref https://www.midjourney.com/jobs/c93195a9-80f5-4314-b2fd-0f1515ea6d63?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.4.2** — Transformation explosion

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-03 |

```
Close-up torso, massive crystallization surge, flesh rapidly becoming red geometric facets, internal structure becoming visible as ruby crystal, violent transformation wave, body horror maximum, extreme detail shot, harsh dramatic lighting --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 550
```

---

**3.4.3** — Losing human form

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-03 |

```
Medium shot, figure's body now mostly red crystalline, human elements retreating rapidly, original form barely visible, identity almost gone, tragic transformation, Beksinski body horror, dynamic pose of anguish, volumetric red light --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.4.4** — Environment in frenzy

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-03 |

```
Wide shot, red crystalline void in aggressive motion, ruby formations multiplying rapidly, swirling around transforming figure, feeding frenzy of geometry, apocalyptic alien landscape, maximum chaos, extreme wide shot, harsh pulsing crimson light --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 550
```

---

**3.4.5** — Face consumed

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-03 |

```
Extreme close-up, last human eye visible amid red crystalline face, tear falling from human eye, crystal growing over it, final moments of identity visible, intimate horror detail, macro close-up, soft focus on tear sharp on crystal growth --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.4.6** — Final human trace

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-03 |

```
Close-up hand, single finger still flesh reaching toward mirror, rest of hand red crystal, last human element, desperate reaching, beautiful tragic detail, intimate body horror, extreme close-up, dramatic contrast lighting --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**3.4.7** — Complete transformation

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-03 |

```
Medium shot, figure now entirely red crystalline, humanoid shape made of ruby geometric facets, no flesh remains, new form stands where human was, identity completely consumed, beautiful horrible completion, full body shot, volumetric crimson light --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.4.8** — New being

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-03 |

```
Wide shot, red crystalline humanoid stands in ruby geometric void, indistinguishable from environment, became what consumed them, part of the Other now, vast crimson landscape and figure as one, cinematic wide shot, ambient red glow --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 450
```

---

## Scene 3.5: What Remains — VERSE (2:05 - 2:20) — 4 images

---

**3.5.1** — Examining new form

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-02 |

```
Medium shot, red crystalline being examines own faceted hands, trying to understand what they've become, ruby geometry where flesh was, alien to themselves, quiet horror of completion, soft red ambient lighting, experimental anime aesthetic --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/2d500449-a6a6-4853-ad4e-1d5470f49845?index=1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**3.5.2** — Memory of flesh

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-02 |

```
Close-up crystalline face, faceted ruby features trying to form human expression, ghost of former self visible in geometry, identity struggling within crystal prison, haunting detail, intimate portrait of loss, soft volumetric red light --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/2d500449-a6a6-4853-ad4e-1d5470f49845?index=1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**3.5.3** — Part of the environment

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-02 |

```
Wide shot, red crystalline being walks through ruby void, movement matching the environment's rhythm, becoming one with the Other, assimilation visible, figure and landscape harmonizing, vast crimson geometric space, cinematic wide shot, ambient red glow --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/2d500449-a6a6-4853-ad4e-1d5470f49845?index=1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**3.5.4** — The final mirror

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-02 |

```
Medium shot, red crystalline being discovers ornate mirror floating in void, different from others, special, drawn toward it with purpose, approaching revelation, dramatic lighting from mirror surface, anticipation building --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/2d500449-a6a6-4853-ad4e-1d5470f49845?index=1 --sw 100 --ar 16:9 --v 7 --s 350
```

---

## Scene 3.6: Third Acceleration — CHORUS (2:20 - 2:30) — 6 images

---

**3.6.1** — Approaching truth

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-03 |

```
Medium shot, red crystalline being approaches final mirror rapidly, environment pulsing with energy, moment of revelation imminent, ruby figure against reflective surface, dramatic movement toward truth, harsh crimson lighting --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.6.2** — Environment responds

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-03 |

```
Wide shot, entire red crystalline void shifts toward the mirror, ruby geometry orienting to witness, massive environmental change, the Other watching through itself, vast crimson landscape in motion, chaotic dynamic composition --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 550
```

---

**3.6.3** — Looking in

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-03 |

```
Over-shoulder shot, red crystalline being looks into mirror, reflection not yet revealed to viewer, figure sees something shocking, body language of horror, dramatic moment before reveal, tense composition, harsh lighting contrast --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**3.6.4** — The truth

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | OTHER-03 |

> **IMPORTANT:** This shows the ORIGINAL human self trapped IN the mirror!

```
Close-up mirror surface, reflection shows ORIGINAL HUMANOID SELF trapped INSIDE the mirror, flesh and blood human form with porcelain skin and golden chest glow pressed against glass from within, screaming silently, warm human trapped in cold reflection, the transformation revealed as exchange, horrific revelation, extreme close-up of mirror --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.6.5** — Reversal revealed

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-03 |

> **NOTE:** This shows BOTH - crystalline being outside, human trapped inside. Generate separately if needed.

```
Wide shot showing both: red crystalline being standing OUTSIDE mirror looking in, original warm human self visible trapped INSIDE mirror reaching out, roles reversed, outside became inside, watcher became watched, devastating composition, harsh dramatic lighting, split between crimson and warm gold --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**3.6.6** — Mutual horror

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-03 |

```
Split composition, red crystalline being on left reaching toward mirror in horror, trapped human self visible in mirror on right reaching back from inside, both in anguish, same gesture opposite sides of glass, symmetric tragedy, dramatic contrasting light warm and cold --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 500
```

---

# ACT 4: THE REALIZATION (2:30 - 3:00)
*Peak horror — Maximum intensity*

## Scene 4.1: Trapped Self (2:30 - 2:45) — 8 images

---

**4.1.1** — The prison

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | OTHER-03 |

> **IMPORTANT:** Focus on the trapped HUMAN self inside the mirror

```
Close-up mirror surface, original humanoid self trapped within, pressing pale hands against glass from inside, flesh and golden warmth imprisoned in reflection, expression of absolute terror, trapped in own reflection, porcelain skin warm light, intimate horror portrait, soft warm light inside cold frame --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**4.1.2** — Desperate eyes

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | — |

```
Extreme close-up, human eye seen through mirror glass, tear rolling down cheek, desperation and horror in gaze, trapped soul looking out from within reflection, intimate devastating detail, the watched becomes watcher from inside, macro detail shot, soft focus on glass sharp focus on eye --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --ar 16:9 --v 7 --s 400
```

---

**4.1.3** — Pounding glass

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | — |

```
Medium shot inside mirror perspective, trapped humanoid self pounds fists against glass barrier from within, expression of anguish and desperation, trying to break free, warm golden light illuminates flesh from within prison, confined desperation, dynamic pose, dramatic internal lighting --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --ar 16:9 --v 7 --s 450
```

---

**4.1.4** — Outside horror

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-03 |

```
Medium shot, red crystalline being stands frozen before mirror, faceted ruby form showing horror through geometry, realizing what they've become and what they've lost, confronting the exchange, horrific self-recognition, dramatic red lighting --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 450
```

---

**4.1.5** — Hands almost touching

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-03 |

```
Close-up hands, red crystalline faceted hand presses against mirror from outside, flesh hand with warm skin presses from inside, almost touching through glass, cannot connect, same person separated by transformation, devastating detail, intimate tragedy, harsh lighting contrast between warm and cold --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**4.1.6** — Screaming inside

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | — |

```
Close-up through mirror glass, trapped human self screaming silently inside reflection, mouth open in despair, sound cannot escape the glass, imprisoned in own reflection forever, intimate horror, extreme close-up through distorting glass surface, warm light trapped within --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --ar 16:9 --v 7 --s 450
```

---

**4.1.7** — Crystal weeping

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-03 |

```
Extreme close-up, red crystalline face of being outside mirror, ruby facets somehow expressing grief through geometry, crimson tear-like formations at eye area, monster mourning its lost humanity, beautiful horrible detail, macro shot, soft red light --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**4.1.8** — The divide

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-03 |

```
Wide shot, red crystalline being and mirror with trapped warm human self visible within, vast ruby void surrounding, isolation of transformation complete, two versions of same person eternally separated, devastating composition, cinematic wide shot, dramatic volumetric red light contrasting warm mirror glow --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 450
```

---

## Scene 4.2: Desperate Reaching (2:45 - 3:00) — 8 images

---

**4.2.1** — Trying to break through

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-03 |

```
Medium shot, red crystalline being claws at mirror surface desperately, trying to break through to trapped self, desperate violent attempt, ruby hands scraping against glass, futile rescue attempt, dynamic aggressive pose, harsh dramatic lighting --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**4.2.2** — Cracks forming

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-03 |

```
Extreme close-up, cracks spreading through red crystalline being's hands from effort of reaching, the attempt to reunite destroys them, ruby facets fracturing and splintering, self-destruction through desperation, detailed body horror, macro shot of cracking crystal --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**4.2.3** — Inside reaching back

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | — |

```
Close-up from inside mirror perspective, trapped human self reaching toward glass, toward the crystalline being that was once them, pale hands pressed against barrier, desperation matching desperation outside, two halves yearning for impossible reunion, warm hands against cold glass, emotional intimate shot --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --ar 16:9 --v 7 --s 450
```

---

**4.2.4** — Being fractures

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-03 |

```
Medium shot, cracks spreading up red crystalline being's arms from strain of reaching, body beginning to fragment from effort, the cost of desperate reaching, destruction accelerating, ruby form failing, dynamic pose of deterioration, harsh crimson lighting --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**4.2.5** — Environment reacts

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-03 |

```
Wide shot, red crystalline void churns aggressively around scene, ruby geometry responding to the fracturing being, the Other disturbed by destruction of its absorbed part, chaotic environmental response, vast crimson chaos, extreme wide shot, harsh dynamic lighting --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 550
```

---

**4.2.6** — Pressing harder

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-03 |

```
Close-up, red crystalline being presses faceted face against mirror surface, features distorting against glass, trying to be closer to trapped self, desperate intimacy, face cracking from pressure, devastating detail, extreme close-up, harsh lighting --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**4.2.7** — Watching self break

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | — |

```
Medium shot from inside mirror perspective, trapped human self watches their crystalline form fracturing outside the glass, horror at watching own destruction from within, helpless witness, confined viewer watching inevitable collapse, dramatic perspective from within mirror, warm light contrasting cold exterior --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --ar 16:9 --v 7 --s 450
```

---

**4.2.8** — Point of shattering

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-03 |

```
Wide shot, red crystalline being covered in fracture lines, moments from total collapse, still reaching desperately for mirror, ruby form about to shatter completely, final desperate gesture before destruction, tragic pre-destruction pose, dramatic crimson lighting, tense stillness before breaking --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0 --sw 100 --ar 16:9 --v 7 --s 500
```

---

# ACT 5: SHATTERING (3:00 - END)
*Falling action — Slowing pace*

## Scene 5.1: The Breaking (3:00 - 3:12) — 5 images

---

**5.1.1** — First shattering

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-04 |

```
Medium shot, red crystalline being SHATTERS starting from reaching hand, ruby fragments explode outward in beautiful destruction, body breaking into geometric pieces, the cost of yearning for what was lost, dynamic explosive composition, harsh dramatic lighting with motion blur --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/44db4e65-7465-45b3-a990-5173111cdd38?index=1 --sw 100 --ar 16:9 --v 7 --s 550
```

---

**5.1.2** — Cascade of fragments

| Reference | Image |
|-----------|-------|
| OREF | SELF-04 |
| SREF | OTHER-04 |

```
Wide shot, red crystalline body fragmenting rapidly into countless pieces, ruby shards scatter in all directions, form dissolving completely, beautiful horrible dissolution, geometric rain of what was once a being, vast void filling with crimson fragments, chaotic wide shot, volumetric red light --oref https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0 --ow 200 --sref https://www.midjourney.com/jobs/44db4e65-7465-45b3-a990-5173111cdd38?index=1 --sw 100 --ar 16:9 --v 7 --s 500
```

---

**5.1.3** — Watching destruction

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | — |

```
Close-up from inside mirror, trapped human self watches crystalline body shatter outside the glass, expression of grief and horror, witnessing their own death from within prison, tears streaming, devastated witness to inevitable, intimate emotional shot through glass surface, warm tears cold exterior --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --ar 16:9 --v 7 --s 450
```

---

**5.1.4** — Fragments floating

| Reference | Image |
|-----------|-------|
| OREF | — |
| SREF | OTHER-04 |

```
Wide shot, countless red crystalline shards floating through vast void, what was once a being now scattered geometry, beautiful dissolution complete, ruby pieces drift slowly and peacefully, environment begins absorbing them, vast crimson void with floating fragments, peaceful aftermath of destruction, soft ambient red light --sref https://www.midjourney.com/jobs/44db4e65-7465-45b3-a990-5173111cdd38?index=1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**5.1.5** — Environment absorbing

| Reference | Image |
|-----------|-------|
| OREF | — |
| SREF | OTHER-04 |

```
Medium shot, red crystalline void absorbs floating fragments, ruby geometry consuming shattered pieces, the Other reclaiming what it made, fragments dissolving into larger formations, assimilation complete, the environment feeds, soft flowing absorption motion, ambient crimson glow --sref https://www.midjourney.com/jobs/44db4e65-7465-45b3-a990-5173111cdd38?index=1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

## Scene 5.2: Into the Void (3:12 - 3:22) — 4 images

---

**5.2.1** — Last fragments

| Reference | Image |
|-----------|-------|
| OREF | — |
| SREF | OTHER-04 |

```
Wide shot, final red crystalline fragments float through vast void, almost all absorbed by environment, sparse ruby pieces remaining, peaceful ending of dissolution, vast empty crimson space, minimal composition, soft ambient light fading slowly --sref https://www.midjourney.com/jobs/44db4e65-7465-45b3-a990-5173111cdd38?index=1 --sw 100 --ar 16:9 --v 7 --s 350
```

---

**5.2.2** — Mirror alone

| Reference | Image |
|-----------|-------|
| OREF | — |
| SREF | OTHER-02 |

```
Wide shot, single ornate mirror floats alone in red crystalline void, only artifact remaining in vast space, surrounding ruby geometry pulses slowly with satisfied rhythm, isolated object in infinite crimson space, ominous solitude, cinematic wide shot, soft ominous red glow --sref https://www.midjourney.com/jobs/2d500449-a6a6-4853-ad4e-1d5470f49845?index=1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**5.2.3** — Trapped forever

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | OTHER-02 |

```
Close-up of mirror floating in void, trapped human self still visible inside, pressing against glass with eternal despair, prisoner in own reflection forever, no rescue coming ever, devastating final portrait of the trapped soul, intimate close-up, soft warm light trapped in cold frame surrounded by red void --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --sref https://www.midjourney.com/jobs/2d500449-a6a6-4853-ad4e-1d5470f49845?index=1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

**5.2.4** — Final image

| Reference | Image |
|-----------|-------|
| OREF | SELF-01 |
| SREF | OTHER-02 |

```
Wide establishing shot, mirror floating in infinite red crystalline void, trapped human self visible small within pressing against glass, vast ruby geometric environment surrounding and watching and pulsing, the Other victorious forever, eternal imprisonment complete, final haunting composition, cinematic wide shot, soft pulsing crimson light --oref https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2 --ow 200 --sref https://www.midjourney.com/jobs/2d500449-a6a6-4853-ad4e-1d5470f49845?index=1 --sw 100 --ar 16:9 --v 7 --s 400
```

---

## Scene 5.3: Fade (3:22 - END) — 3 images

---

**5.3.1** — Environment pulses

| Reference | Image |
|-----------|-------|
| OREF | — |
| SREF | OTHER-02 |

```
Wide shot, red crystalline void pulses slowly with satisfied rhythm, vast ruby geometry breathing contentedly after feeding, the Other satiated, mirror tiny in far distance, peaceful apocalyptic landscape at rest, serene horror, soft rhythmic crimson light --sref https://www.midjourney.com/jobs/2d500449-a6a6-4853-ad4e-1d5470f49845?index=1 --sw 100 --ar 16:9 --v 7 --s 350
```

---

**5.3.2** — Darkness creeping

| Reference | Image |
|-----------|-------|
| OREF | — |
| SREF | — |

```
Wide shot, edges of red crystalline void fading to black, darkness consuming the crimson from all sides, light dying slowly, reality ending, fade to void beginning, vast space diminishing, creeping absolute darkness from edges, soft dying red glow --ar 16:9 --v 7 --s 350
```

---

**5.3.3** — Final black

| Reference | Image |
|-----------|-------|
| OREF | — |
| SREF | — |

```
Nearly black frame, last traces of red crystalline light fading to nothing, void consuming all color, only faint suggestion of ruby glow remaining then gone, ending, darkness wins, minimal abstract composition, almost pure black with dying crimson whispers --ar 16:9 --v 7 --s 300
```

---

# QUICK REFERENCE: WHICH IMAGE FOR EACH SCENE

## THE SELF (--oref)

| Act/Scene | Reference | Reason |
|-----------|-----------|--------|
| ACT 1 (all) | SELF-01 | Intact human |
| ACT 2 (all) | SELF-01 | Still intact |
| 3.1 | SELF-02 | Early deterioration |
| 3.2 | SELF-03 | Mid-transformation chorus |
| 3.3 | SELF-03 | Mid-transformation verse |
| 3.4 (early) | SELF-03 | Transitioning |
| 3.4 (late) | SELF-04 | Near complete |
| 3.5 | SELF-04 | Crystalline form |
| 3.6 | SELF-04 + SELF-01 | Both forms (revelation) |
| ACT 4 (outside) | SELF-04 | Crystalline being |
| ACT 4 (trapped) | SELF-01 | Human in mirror |
| ACT 5 | SELF-04 + SELF-01 | Shattering + trapped |

## THE OTHER Environment (--sref)

| Section | Reference | Reason |
|---------|-----------|--------|
| Verses (slow) | OTHER-01 or OTHER-02 | Peaceful/Active |
| Choruses (fast) | OTHER-03 | Aggressive |
| Climax (ACT 4) | OTHER-03 | Maximum intensity |
| Shattering | OTHER-04 | Apocalyptic |
| Ending fade | OTHER-02 → none | Calming to black |

---

# TOTAL IMAGE COUNT: 78 images

| Act | Images | Character Refs Used |
|-----|--------|---------------------|
| ACT 1 | 12 | SELF-01 |
| ACT 2 | 8 | SELF-01 |
| ACT 3 | 35 | SELF-02 → SELF-03 → SELF-04 |
| ACT 4 | 16 | SELF-04 + SELF-01 |
| ACT 5 | 7 | SELF-04 + SELF-01 |

---

# PRODUCTION CHECKLIST

```
STEP 1 - CREATE REFERENCE IMAGES:
[X] SELF-01 generated and URL saved: https://www.midjourney.com/jobs/74d0e64d-5307-4035-934e-6ff290fa3351?index=2
[X] SELF-02 generated and URL saved: https://www.midjourney.com/jobs/f635f459-9a5c-452e-894f-28b1201814eb?index=0
[X] SELF-03 generated and URL saved: https://www.midjourney.com/jobs/c93195a9-80f5-4314-b2fd-0f1515ea6d63?index=0
[X] SELF-04 generated and URL saved: https://www.midjourney.com/jobs/daefa63d-ae7d-42f8-ab8c-b8f1e0185045?index=0
[X] OTHER-01 generated and URL saved: https://www.midjourney.com/jobs/104deaa1-7824-4248-8aad-62a240b8130c?index=2
[X] OTHER-02 generated and URL saved: https://www.midjourney.com/jobs/2d500449-a6a6-4853-ad4e-1d5470f49845?index=1
[X] OTHER-03 generated and URL saved: https://www.midjourney.com/jobs/636c8236-6108-4db2-bfb0-9131c51b2d07?index=0
[X] OTHER-04 generated and URL saved: https://www.midjourney.com/jobs/44db4e65-7465-45b3-a990-5173111cdd38?index=1

STEP 2 - GENERATE SCENE IMAGES:
[ ] ACT 1 Scene 1.1 (4 images)
[ ] ACT 1 Scene 1.2 (4 images)
[ ] ACT 1 Scene 1.3 (4 images)
[ ] ACT 2 Scene 2.1 (5 images)
[ ] ACT 2 Scene 2.2 (3 images)
[ ] ACT 3 Scene 3.1 VERSE (5 images)
[ ] ACT 3 Scene 3.2 CHORUS (8 images)
[ ] ACT 3 Scene 3.3 VERSE (4 images)
[ ] ACT 3 Scene 3.4 CHORUS (8 images)
[ ] ACT 3 Scene 3.5 VERSE (4 images)
[ ] ACT 3 Scene 3.6 CHORUS (6 images)
[ ] ACT 4 Scene 4.1 (8 images)
[ ] ACT 4 Scene 4.2 (8 images)
[ ] ACT 5 Scene 5.1 (5 images)
[ ] ACT 5 Scene 5.2 (4 images)
[ ] ACT 5 Scene 5.3 (3 images)

STEP 3 - POST-PRODUCTION:
[ ] Import all 78 images to DaVinci Resolve
[ ] Arrange in sequence order
[ ] Sync to music beats
[ ] Add Ken Burns pan/zoom effects
[ ] Add transitions (dissolves for verses, hard cuts for choruses)
[ ] Color grade for consistency
[ ] Export final video
```

---

# SOURCES

- [Midjourney Omni Reference Guide](https://www.cometapi.com/how-to-use-omni-reference-in-midjourney-v7/)
- [Midjourney Character Consistency - AIArty](https://www.aiarty.com/midjourney-guide/midjourney-consistent-character.htm)
- [Midjourney V7 Prompting - SurePrompts](https://sureprompts.com/blog/midjourney-v7-prompting-guide)
- [Style Reference Guide - SkyWork](https://skywork.ai/skypage/en/Mastering-Midjourney-sref-The-Ultimate-Guide-to-Consistent-and-Stunning-AI-Art/1976164257333571584)

---

# THE STORY (REPEATED FOR REFERENCE)

**"Selfless" = Becoming SELF-LESS (empty, no identity)**

THE SELF is a humanoid being searching for their reflection in an infinite mirror labyrinth. But every mirror shows something wrong — not their face, but glimpses of a red crystalline void. THE OTHER is not a character but the environment itself: a living, breathing red crystalline dimension that watches, waits, and hungers.

Drawn by obsession, THE SELF steps through a mirror and enters this crimson geometric world. At first it's peaceful, beautiful, seductive. But the environment begins to consume them. Their flesh cracks. Crystals grow from their skin. With each verse, the change creeps slowly. With each chorus, it accelerates violently.

THE SELF explores deeper, hoping to find themselves, but only loses more. The red crystalline environment shifts and morphs constantly — it IS the Other, surrounding them completely, absorbing them piece by piece.

In the climax, THE SELF finds one final mirror. They look in and see the horror: they have BECOME part of the red crystalline environment. Their old human self is trapped IN the mirror, looking back, screaming silently. The watcher has become the watched. The consumed has become the consumer.

Desperate, the now-crystalline being reaches for the mirror, trying to touch their old self. But the strain shatters them. They fragment into a thousand red crystalline shards, scattering into the void. The environment — THE OTHER — absorbs these pieces.

Final image: the mirror floats alone in the red crystalline void. Inside it, the trapped human SELF presses against the glass forever. The environment pulses. It has won. It has always won.

**The message:** When you give yourself completely to another, you don't just lose yourself — you become the thing that consumed you, and your true self becomes a prisoner you can never reach again.
