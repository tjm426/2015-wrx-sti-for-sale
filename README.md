# 2015 Subaru WRX STI Limited — For Sale Listing

Static one-page car listing site. Drop into any static host (Netlify Drop, GitHub Pages, etc.).

---

## Setup Checklist

### 1. Add your photos

Create a `photos/` folder next to `index.html` and drop your images in. Then replace the placeholder `<div>` blocks in the **Photos** section of `index.html` with actual `<img>` tags:

```html
<img src="photos/front-34.jpg" alt="Front 3/4 view" />
<img src="photos/rear-34.jpg" alt="Rear 3/4 view" />
<!-- etc. -->
```

**Hero image:** Name your best exterior shot `photos/hero.jpg` and add this to the `<style>` block (or inline on `.hero-photo`):

```css
.hero-photo {
  background-image: url('photos/hero.jpg');
}
```

Recommended shots (in priority order):
- Front 3/4 (hero candidate)
- Rear 3/4
- Both sides straight-on
- Engine bay
- Interior / dash
- Odometer showing ~70k
- Wheels close-up
- Any imperfections (builds trust)

### 2. Set your asking price

Find this line in `index.html` and replace `$XX,XXX`:

```html
<div class="price-tag">$XX,XXX</div>
```

### 3. Add your contact info

Find the two anchor tags near the bottom and update:

```html
<a class="contact-btn" href="tel:+19705550000">Call or Text</a>
<a class="contact-btn" href="mailto:you@email.com">Email</a>
```

### 4. Update the listing description

In the **About This Car** section, fill in:
- Service history highlights
- Any recent maintenance (tires, brakes, fluids, etc.)
- Carfax availability

### 5. Review the features list

The `<ul class="feature-list">` is pre-filled with standard STI Limited features. Remove anything that doesn't apply, add anything notable.

---

## Deploying

### Netlify Drop (fastest)
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag the entire folder (with `photos/` subfolder) onto the page
3. Live in ~30 seconds — you'll get a URL like `https://random-name.netlify.app`

### GitHub Pages
```bash
git init
git add .
git commit -m "Initial listing"
gh repo create sti-listing --public --source=. --push
# Then enable Pages in repo Settings → Pages → Deploy from branch: main / root
```

---

## Listing Platforms to Link This From

| Platform | Notes |
|---|---|
| **BringATrailer.com** | Best for enthusiasts, often above-market prices |
| **Cars & Bids** | Similar to BaT, good for enthusiast vehicles |
| **Facebook Marketplace** | Great for local CO buyers |
| **r/WRX / r/Spoolies** | Active Subaru communities, free |
| **Craigslist** | Still works for local |

---

## Car Details (reference)

| Field | Value |
|---|---|
| Year | 2015 |
| Make/Model | Subaru WRX STI |
| Trim | Limited |
| Mileage | ~70,000 |
| Color | Dark Gray Metallic |
| Engine | 2.5L Turbocharged Boxer (EJ257) |
| Power | 305 hp |
| Drivetrain | Symmetrical AWD |
| Transmission | 6-Speed Manual |
| Location | Loveland, CO 80538 |
