# rank-cat-photo-spontaneity

Ranks a collection of cat photographs by their **spontaneous aliveness** — the degree to which each image feels like a fleeting moment seized from the flow of ordinary life, rather than a carefully constructed composition.

## Input

An array of two or more cat photograph images. No metadata, captions, or camera settings are required — the function evaluates only what the image itself communicates.

```
[image, image, image, ...]
```

## Output

A vector of scores (one per input image) that sum to approximately 1. Higher scores indicate greater spontaneous aliveness. The scores define a relative ranking: photographs that radiate the energy of a captured accident score highest, while photographs that feel engineered or overproduced score lowest, regardless of their technical polish.

## What It Evaluates

The function assesses three distinct qualities across every photograph. Together, these qualities answer one central question: **was this photograph an event or an artifact?**

### 1. Temporal Urgency

Does this moment feel like it almost wasn't captured? The function looks for signs that the shutter clicked just in time — motion blur from a body moving faster than the camera can freeze, the explosive geometry of a cat mid-leap or mid-pounce, a wide-eyed expression caught in the instant before it changed, or any posture so precarious it could only have lasted a fraction of a second. Images where the viewer instinctively feels that one moment later this scene no longer existed score high. Images where the cat is still and settled — capturable at any point over a long window of time — score low.

### 2. Uncomposed Framing

Does the composition reveal a photographer reacting on instinct rather than deliberately designing an image? The function looks for the hallmarks of a grab shot: the cat clipped at the edges of the frame, the subject off-center or in an unexpected region of the image, an awkward shooting angle, a slight tilt, or focus that landed imperfectly because there was no time to adjust. These imperfections are treated as evidence of authenticity. Conversely, deliberate rule-of-thirds placement, carefully chosen shallow depth of field, flattering angles, and clean intentional edges signal that the photographer had time to compose — and the image scores lower accordingly.

### 3. Environmental Authenticity

Does the setting reflect the unedited texture of real everyday life? The function looks for the honest clutter of a home shared with a cat — rumpled blankets, visible household objects, harsh or uneven natural lighting, ordinary furniture, and the general imperfection of a space that has not been tidied for the camera. These details signal that the photograph was pulled from the flow of an ordinary day. Clean minimal backdrops, studio lighting, artfully arranged props, or backgrounds that have been deliberately composed to flatter the subject all indicate curation or staging, and the image scores lower.

## Use Cases

- **Social media platforms** surfacing authentic, candid cat content over manufactured influencer imagery
- **Cat adoption services** selecting photos where prospective owners can see a cat being genuinely itself, rather than posed in sterile portrait settings
- **Photography communities** celebrating the decisive moment — the Cartier-Bresson instinct of firing the shutter at exactly the right instant — over meticulous post-production
- **Personal photo libraries** rediscovering the best spontaneous memories from years of living with a cat, filtering past posed holiday photos to find the chaotic, joyful, real ones
- **Content curation pipelines** that need to programmatically distinguish candid photography from staged or professional imagery

## Philosophy

The function does not penalize beauty. A cat caught mid-leap in a shaft of golden afternoon light, blurred and off-center and surrounded by the clutter of a living room, can be breathtaking. What the function penalizes is **control** — the visible hand of a photographer who had enough time and authority over the scene to make it perfect. Perfection is treated as evidence: it tells us the moment was not fleeting, not seized, not rescued from the edge of disappearing. What rises to the top is something harder to manufacture and more honest in its beauty — the photograph that carries within it the urgency of its own creation.