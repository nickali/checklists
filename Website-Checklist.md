# Website Checklist

## Front-End Checklist

### Head

* [ ] **Doctype:** Set Doctype to HTML5 and is at the top of all HTML pages.
* [ ] **Charset:** Set to UTF-8.
* [ ] **X-UA-Compatible:**  Set X-UA-Compatible meta tag.
* [ ] **Viewport:**  Set viewport.
* [ ] **Favicons:**  Set favicon file location.
* [ ] **Apple Touch & Android Icons:**  Set Apple touch & Android icons.
* [ ] **Canonical:**  Set ``rel=“canonical”``.
* [ ] **Smart App Banner:** Set app-id and app-argument

### HTML tags

* [ ] **Language tag:**  Set language tag.
* [ ] **Conditional comments:**  Set conditional comments for IE if necessary.
* [ ] **RSS feed:**  Set RSS URL if needed.

### Social meta

* [ ] **Facebook Open Graph:** Set including images.
* [ ] **Twitter Card:** Set including images.

—

## HTML

### Best practices

* [ ] **HTML5 Semantic Elements:**  Use HTML5 semantic elements appropriately
* [ ] **Error pages:**  Create 404 page and 5xx error pages. 5xx error pages are handled by web server.
* [ ] **Clean up comments:**  Remove unnecessary comments created when building site.
* [ ] **AMP / Instant Articles:** Verify proper generation.

### HTML testing

* [ ] **W3C compliant:**:  Run pages through W3C validato.
* [ ] **Desktop Browsers:**  Test pages on current (and back one version) of current desktop browsers
* [ ] **Mobile Browsers:**   Test pages on current (and back on version) current mobile browsers
* [ ] **Link checker:**  Verify no broken links.
* [ ] **Adblockers test:**  Verify adblockers do not break pages.

—

## Fonts

* [ ] **Webfont format:**  Convert fonts to WOFF, WOFF2 and TTF files.
* [ ] **Fall-back Typefaces:**  List 2 or more for webfonts.
* [ ] **Service Configuration:** Verify live domain white-listed for hosted font services.

—

## CSS

* [ ] **Preprocessors:**  Verify no links to Deb preprocessor paths. 
* [ ] **Breakpoints:** Verify content, flow, and UX work as intended at different breakpoints.
* [ ] **CSS Print:**  Set print stylesheet on each page.
* [ ] **Unique ID:**  Use unique IDs per page.
* [ ] **Reset CSS:** Use CSS reset stylesheet.
* [ ] **JS prefix:**  Name classes or IDs with **js-** when modified by JavaScript and not by CSS files.
* [ ] **CSS embed or line:**  Remove all embedded or inline CSS.
* [ ] **Vendor prefixes:**  Use CSS vendor prefixes depending on required browser support compatibility.

### Performance

- [ ] **Concatenation:**  Concatenate CSS files.
- [ ] **Minification:**  Minify CSS files.
- [ ] **Non-blocking:**  Verify CSS files are non-blocking.
- [ ] **Unused CSS:**  Cleanup CSS.

### CSS testing

* [ ] **CSS Validator:** Verify all CSS is valid.

—

## Images / Videos

### Best practices

* [ ] **Placeholder Images:** Verify all removed
* [ ] **Stock Images:** Verify watermarked images replaced with licensed versions. 
* [ ] **Optimization:**  Verify all images are optimized for respective browsers.
* [ ] **Retina:**  Use x2 or 3x images to support retina display.
* [ ] **Width and Height:**  All ``<img>`` have height and width set or handle globally.
* [ ] **Alternative text:**  All ``<img>`` have an alternative text which describe the image visually.
* [ ] **Lazy loading:**  Load images on scroll or as needed.
* [ ] **Social Thumbnails**: Verify Facebook/Twitter/LinkedIn thumbnails generated for all pages.
* [ ] **Flexible Video:**  Verify videos resize on respective browsers.
* [ ] **Video Controls:** Verify playblack, pause, and mute controls visible.
* [ ] **Filenames:** Verify filenames are keyword friendly.

—

## Copy
* [ ] **Text:** Verify all Lorem Ipsum removed.

—

## JavaScript

### Best practices

* [ ] **JavaScript Inline:**  Remove or minimize inline JavaScript.
* [ ] **Concatenation:**   Concatenate Javascript files.
* [ ] **Minification:** Minify JavaScript files.
* [ ] **Non-blocking:**  Load JavaScript files asynchronously.
* [ ] **Modernizr:**  Use Modernizr or similar tool to test for specific browser features.
* [ ] **Footer Load** Place scripts in footer of page.

### JavaScript testing

* [ ] **ESLint:** Verify JavaScript with ESLint or similar tool.

—

## Security

* [ ] **HTTPS:** User HTTPS
* [ ] **HSTS:** Set HTTP Strict Transport Security parameter on web server.
* [ ] **Cross Site Request Forgery (CSRF):** Scrub and verify inputs, verify headers and use tokens.
* [ ] **Cross Site Scripting (XSS):**  Minimize attack vectors and SQL injection by sanitizing input data and tracking logins and sessions.
* [ ] **Encryption:** Verify passwords, credit card numbers, cookies, etc are hashed and encrypted.
* [ ] **Password Reset:** Verify password rules on all authentication pages like Registration, forgot password, change password
* [ ] **Login Limits:** Require ‘human’ verification.
* [ ] **System Information:** Verify application, server, or database version or information not publicly viewable.
* [ ] **Roles and Rights:** Verify authentication and authorization process.
* [ ] **Address Bar:** Verify encrypted session values in address bar.
* [ ] **SSL** Verify certificate not expiring. 

—

## Performance

### Best practices

- [ ] **Minified:** Minimize HTML and enable gzip type compression on web server.
- [ ] **Lazy loading:** Load images, scripts, and CSS files as needed, not on load.
- [ ] **Cookie size:** Minimize size of cookies.
- [ ] **Content Delivery Network:** Push CSS, JavaScript, fonts, and generated HTML to CDN.
- [ ] **HTTP Cache Headers:** Set approriate parameters.
- [ ] **DNS Prefetching:** Verify ``preload`` and/or ``dns-prefetch`` enabled.
- [ ] **Mixed Content:** Verify all assets retrievalbe using HTTPS.
- [ ] **Logging:** Verify tools enabled and passing data to monitoring platforms.

—

## SEO

* [ ] **Indexing:** Enable search engines to index site.
* [ ] **Tag Manager:** Verify proper installation.
* [ ] **Analytics & Conversion:**  Google Analytics or similar tools is installed and correctly configured.
* [ ] **Ad Pixels:** Verify all ad pixels installed and registering.
* [ ] **Heatmaps**: Verify installation of SaaS tool.
* [ ] **Chat:**: Verify chat installation.
* [ ] **Headings logic:**  Heading text helps to understand the content in the current page.
* [ ] **Sitemap XML:** Site, image, and video XMLs generated and submitted to Google Webmaster Tools and similar tools
* [ ] **robots.txt:** Verify robots.txt not blocking any pages.
* [ ] **Structured Data or Rich Snippets:**  Generate error-free structured data as needed.
* [ ] **Title:**  Unique title tag used on each page.
* [ ] **Description:**  Set unique meta description on each page.
* [ ] **301 Redirects:** Moved content should return 301 to browser.
* [ ] **Title Attribute**: Verify all links have ``title`` attribute set.
* [ ] **Social Widgets:** Verify buttons / links showing in right palces.

—

## Legal

* [ ] **Privacy Policy:**  Verify link visible in footer and page exists.
* [ ] **Terms of Service:**  Verify link visible in footer and page exists
* [ ] **GDPR Compliance:** Verify consent notice visible.
* [ ] **Copyright** Verify visible in footer. 
—

## Prelaunch

* [ ] **Backups:** Verify backup and restore systems functional.
* [ ] **Versioning:** Verify production code branched or tagged in version control system.
* [ ] **Contact Forms:** Verify CAPTCHA functionality and information emailed or pushed to CRM.
* [ ] **Newsletter Forms** Verify signup forms functional. 
* [ ] **Comments:** Verify moderation notices sent to appropriate email addresses
* [ ] **Search:** Verify CMS search or Google custom search returning correct results.
* [ ] **API Configuration:** Verify live domain witelisted for third party intergrations or SaaS tools.
* [ ] **Dev Domains:** Verify database and assets not referencing dev, staging, or QA environments.
* [ ] **DNS:** Verify proper set up.
* [ ] **Conversions & Funnels:** Verify analytics tools collecting and registering visitor clickstream.
* [ ] **Payment System:** Verify test mode off and transactions work. 
* [ ] **www / non-www:** Verify non-canonical redirects to canonical preserving URL. 

—

## Post Deployment

* [ ] **Baselines:** Create baselines for appropriate metrics like conversions
* [ ] ​

social widgets


—

## WordPress

* [ ] **.htaccess:** Verify file contains correct settings. 
* [ ] **Navigation** Verify navigation works from all pages
* [ ] **Pagination** Verify next and previous links go to right content
* [ ] **Database Table Prefix:** Change from wp_. 
* [ ] **Plugins:** Remove unused plugins. 
* [ ] **Themes:** Remove unused themes. 
* [ ] **Version:** Remove generator meta in header. 
* [ ] **Admin Account:** Rename from admin.
* [ ] **Security Key:** Change from default. 
* [ ] **Admin URL:** Change from default. 