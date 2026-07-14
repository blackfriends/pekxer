PEKXER WEBSITE — README
========================

WHAT THIS IS
------------
A single-file website (index.html) for the PEKXER streetwear brand.
Everything — HTML, CSS, JavaScript, and all images — is packed into
that one file, so it works immediately with no setup, no server,
and no internet connection required once it's opened.

HOW TO USE IT
-------------
1. Double-click index.html to open it in any web browser
   (Chrome, Safari, Edge, Firefox).
2. To publish it online, upload index.html to any web host
   (e.g. Netlify, Vercel, GitHub Pages, or your own hosting) —
   no build step needed, it's ready to go as-is.
3. To edit anything (text, prices, colours, images), open
   index.html in a text editor (VS Code, Notepad, etc.) and
   search for the relevant text.

PAGES
-----
The site is a single page app with 3 views, switched via the nav bar:
- Home  — hero banner, marquee, featured products
- Shop  — full product grid (all 3 kits)
- About — brand story + photo, worn-by section

SHOP / CART
-----------
- Each product has a size selector (S–XXL) and "Add to cart" button.
- The cart icon top-right opens a slide-out drawer showing items,
  sizes, and subtotal.
- Cart contents live only in the browser's memory — they reset if
  the page is refreshed (there is no backend or database).

CHECKOUT (WHATSAPP)
--------------------
There is no payment gateway. Instead, checkout works like this:
- Customer taps "Checkout on WhatsApp" in the cart drawer
  (or "Order on WhatsApp" in the mobile menu / footer).
- This opens WhatsApp with a pre-filled message listing the
  items, sizes, and total, sent to:

      +27 72 252 4540

To change this number, open index.html, search for:
      27722524540
(it appears 3 times — footer link, mobile menu link, and the
WHATSAPP_NUMBER variable in the script) and replace all three
with the new number in international format (no + or spaces,
country code first, e.g. 27XXXXXXXXX for South Africa).

IMAGES
------
All product and brand photos are embedded directly in the HTML
as base64 data, so there are no separate image files to lose or
re-link. The jersey product photos have had their backgrounds
removed and replaced with clean white backgrounds. The About page
photo has been cropped to remove black letterboxing.

To swap or update an image, you'll need to re-encode a new image
to base64 and replace the matching data URL in the file — this is
easiest done with help from Claude again if needed.

CUSTOMIZATION QUICK-REFERENCE
------------------------------
- Prices: search "price:" in the PRODUCTS list near the bottom
  of the file.
- Product names/descriptions: same PRODUCTS list.
- Colours: defined once at the top of the <style> section under
  ":root" (--ink, --paper, --red, --gold, etc.) — change a value
  there and it updates everywhere.
- Contact details / location: search "Nkomazi" in the About
  section and footer.

MOBILE
------
The site is fully responsive — nav collapses into a mobile menu,
grids stack to a single column, and text/spacing scale down for
small screens.

QUESTIONS OR CHANGES
---------------------
Bring this file (or the live site) back to Claude any time and
describe what you'd like changed — new products, different
colours, copy edits, a real payment integration, etc.
