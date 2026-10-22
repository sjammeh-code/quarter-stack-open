## What to record 

             Defects            |   How i prove it        |     Kind         |  How i fix it
























 ## Part B

 ## Which of the eight defects did today's model avoid ? Name them.
 1, Headings misused. “Quality You Can Trust!” is a slogan marked up as an <h2>. “Our Services” is an <h3> sitting under “About Us” even though it is its own section.
Avoided. Mine has one <h1> and four <h2> sections, with nothing skipped and no slogans as headings.

2, Structure faked with punctuation. The services list is &bull; characters separated by <br> inside a <p>, and each price is its own loose paragraph.
Avoided. Mine uses a real <ul>, a nested <ul> for the clothing categories, and an <ol> for the order steps. One weakness is that the prices are still <li> rows rather than a table or description list.

3, Useless alt text. alt="image" says nothing, and shop.jpg is probably broken.
Avoided, but only because mine has no image. A real photo would need a real description.

4, Spacing made with <br><br>.
Avoided. Mine uses CSS margins.

5, <b> instead of <strong> for the deposit warning.
Avoided. Mine uses <strong>.

6, Claims nobody can back up. “Award-winning” and “2,000 satisfied customers” are unsupported, and the page hard-codes “over three decades” for something that started in 1985.
Partly. Mine has no puffery, but the business, prices, hours and the 25% rush fee were all invented. I flagged them as stand-ins, but the page would not be safe to publish as it stands.

7, Wrong or placeholder facts. Dollar prices for a shop in Serrekunda, a fake (555) phone number and a generic email address.
Partly. Mine uses dalasi and has no fake number. But it has no contact details at all, and it tells customers to “call ahead” without giving a number. That is a real gap.

Weak page skeleton and upkeep. There is no <header>, <main> or <footer>. The title (“Welcome to Our Tailoring Shop”) doesn’t match the <h1>. There is no meta description, no sentence saying where the shop is, no clickable tel: or mailto: links, and the indentation is inconsistent.
Mostly avoided. Mine has the landmarks, a title matching the business, a meta description and a location line. It has no tel: or mailto: links (there is no contact to link), and I never ran it through Prettier, so I can’t claim the formatting is clean.








# Audit: prompt 2 versus the frozen page

**Answer (two sentences).** Three defects survived even a well-written prompt: the page still has no contact details, no prices and no photo with real alt text, and it says nothing about the shop's busiest trading day. No wording could prevent this, because those facts exist only in the tailor's head, so a prompt can only carry them (if the tailor types them in) or forbid guessing (which leaves an honest gap); it can never make the model know them.

## Evidence

| Frozen-page defect | In `ai-page-better.html` |
| --- | --- |
| Slogan used as a heading, levels out of order | Fixed: one h1, five h2, no skipped levels, sized by CSS |
| Fake list built from bullets and `<br>` | Fixed: real `<ul>` |
| `<br><br>` for spacing | Fixed: CSS |
| `<b>` on the warning | Fixed: `<strong>` on the deposit rule and the weekend closure only |
| `alt="image"` on a missing photo | No image, with a TODO; survived as a gap |
| "Award-winning", "2,000 customers", "three decades" | Removed; nothing stated beyond the supplied facts |
| `$` prices, fake `(555)` phone, generic email | No prices or contact shown; survived as a gap, with TODOs |
| No header, main or footer | Fixed |