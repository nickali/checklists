# Website Checklist

## HTML
### Best Practices
* [ ] **HTML5 Semantic Elements:**  Use HTML5 semantic elements appropriately.
* [ ] **Error pages:**  Create 404 page and 5xx error pages. 5xx error pages can be handled by web server.
* [ ] **Clean up comments:**  Remove unnecessary comments created when building site.
* [ ] **AMP / Instant Articles:** Generate stripped down HTML for Google and Facebook.

### Head
* [ ] **Doctype:** Set Doctype to HTML5 and put at the top of all HTML pages.
* [ ] **Charset:** Set to UTF-8.
* [ ] **X-UA-Compatible:**  Set for backwards IE compatibility.
* [ ] **Viewport:**  Set viewport.
* [ ] **Favicons:**  Set favicon file location.
* [ ] **Apple Touch & Android Icons:**  Set Apple touch & Android icons.
* [ ] **Canonical:**  Set ``rel=“canonical”``.
* [ ] **Language tag:**  Set language tag.
* [ ] **Conditional comments:**  Set conditional comments for IE.
* [ ] **RSS feed:**  Set RSS URL.
* [ ] **Smart App Banner:** Set app-id and app-argument.
* [ ] **Facebook Open Graph:** Set and link to images.
* [ ] **Twitter Card:** Set and link to images.

### HTML Testing
* [ ] **W3C Compliance:**:  Run pages through W3C validation tools.
* [ ] **Desktop Browsers:**  Test pages on current (and back one version) of current desktop browsers.
* [ ] **Mobile Browsers:**   Test pages on current (and back on version) current mobile browsers.
* [ ] **Link Checker:**  Run pages through broken link checkers.
* [ ] **Adblockers Test:**  Verify adblockers do not break pages.

—

## Fonts
### Best Practices
* [ ] **Webfont Formats:**  Convert fonts to WOFF, WOFF2 and TTF file formats.
* [ ] **Fall-back Typefaces:**  List 2 or more in case desired fonts not available.
* [ ] **Service Configuration:** Set live domain to be white-listed with hosted font services.

—

## CSS
### Best Practices
* [ ] **Preprocessors:**  Remove links to intermediary preprocessor files. 
* [ ] **Breakpoints:** Check content, flow, and UX work as intended at different breakpoints.
* [ ] **CSS Print:**  Set print stylesheet for each page.
* [ ] **Unique ID:**  Use unique IDs per page.
* [ ] **Reset CSS:** Use CSS reset stylesheet.
* [ ] **JavaScript Prefix:**  Name classes or IDs with **js-** when modified by JavaScript and not by CSS files.
* [ ] **Inline / Embedded CSS:**  Remove or minimize embedded or inline CSS.
* [ ] **Vendor Prefixes:**  Use CSS vendor prefixes depending on required browser support compatibility.

### Performance
- [ ] **Concatenation:**  Concatenate CSS files.
- [ ] **Minification:**  Minify CSS files.
- [ ] **Non-blocking:**  Verify CSS files are non-blocking.
- [ ] **Unused CSS:**  Cleanup CSS.

### CSS Testing
* [ ] **CSS Validator:** Run stylesheets through CSS validators.

—

## Images / Videos
### Best Practices
* [ ] **Placeholder Images:** Replace with real images.
* [ ] **Stock Images:** Replace stock watermarked images replaced with licensed versions. 
* [ ] **Optimization:**  Optimize for needed browsers and devices.
* [ ] **Retina:**  Use x2 or 3x images to support retina display.
* [ ] **Width and Height:**  Set ``<img>`` to have height and width, handle with CSS and media queries, or serve appropriate sizes for respective browsers and devices.
* [ ] **Alternative text:**  All ``<img>`` have an alternative text which describe the image visually.
* [ ] **Lazy loading:**  Load images on scroll or as needed.
* [ ] **Social Thumbnails**: Generate Facebook/Twitter/LinkedIn thumbnails for all pages.
* [ ] **Flexible Video:**  Videos resize appropriately on different browsers and devices.
* [ ] **Video Controls:** Show playblack, pause, and mute controls.
—

## Copy
### Best Practices
* [ ] **Text:** Replace all Lorem Ipsum with real copy.

—

## JavaScript
### Best Practices
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
### Best Practices
* [ ] **HTTPS:** Use HTTPS.
* [ ] **HSTS:** Set HTTP Strict Transport Security parameter on web server.
* [ ] **Cross Site Request Forgery (CSRF):** Scrub and verify inputs, verify headers and use tokens.
* [ ] **Cross Site Scripting (XSS):**  Minimize attack vectors and SQL injection by sanitizing input data and tracking logins and sessions.
* [ ] **Encryption:** Hash and encrypt passwords, credit card numbers, cookies, etc.
* [ ] **Password Reset:** Set password rules and flow on all authentication pages like Registration, forgot password, change password.
* [ ] **Login Limits:** Require ‘human’ verification after a defined number of failed tries.
* [ ] **System Information:** Verify application, server, or database version or connection information not publicly viewable.
* [ ] **Roles and Rights:** Verify authentication and authorization process.
* [ ] **Address Bar:** Only show encrypted session values in address bar.
* [ ] **SSL** Verify certificate not expiring. 

—

## Performance
### Best practices
- [ ] **Minified:** Minimize HTML and enable gzip type compression on web server.
- [ ] **Lazy loading:** Load images, scripts, and CSS files as needed, not on load.
- [ ] **Cookie size:** Minimize size of cookies.
- [ ] **Content Delivery Network:** Push CSS, JavaScript, fonts, and generated HTML to CDN.
- [ ] **HTTP Cache Headers:** Set approriate parameters.
- [ ] **DNS Prefetching:** Enable ``preload`` and/or ``dns-prefetch``.
- [ ] **Mixed Content:** Retrieve all files and assets via HTTPS.
- [ ] **Logging:** Enabled tools and verify data passing to monitoring platforms.

—

## SEO
### Best Practices
* [ ] **Indexing:** Enable search engines to index site.
* [ ] **Tag Manager:** Set up and verify data passing to tools.
* [ ] **Analytics & Conversion:**  Google Analytics and similar tools installed,correctly configured, and registering data. 
* [ ] **Ad Pixels:** Verify all ad pixels installed and registering.
* [ ] **Heatmaps**: Verify installation, configuration, and data flow to third party tools.
* [ ] **A/B Tests**: Verify installation, configuration, and data flow to third party tools.
* [ ] **Chat:**: Verify installation, configuration, and data flow to third party tool.
* [ ] **Sitemap XML:** Set up auto-generation and submission of site, image, and video XMLs to Google Webmaster Tools and similar tools
* [ ] **robots.txt:** Verify robots.txt not blocking any pages.
* [ ] **Structured Data or Rich Snippets:**  Generate error-free structured data as needed.
* [ ] **Title:**  Use unique title tag used on each page.
* [ ] **Description:**  Set unique meta description on each page.
* [ ] **301 Redirects:** Return 301 for moved content
* [ ] **Title Attribute**: Set ``title`` attribute for all links.
* [ ] **Social Widgets:** Connect social accounts and set up to show buttons / links in right places.

—

## Legal
### Best Practices
* [ ] **Privacy Policy:**  Create page and put link in footer.
* [ ] **Terms of Service:**  Create page and put link in footer.
* [ ] **GDPR Compliance:** Show consent notice visible.
* [ ] **Copyright** Show in footer. 
—

## Prelaunch
### Best Practices
* [ ] **Backups:** Check backup and restore systems functional.
* [ ] **Versioning:** Branch or tag production code in version control system.
* [ ] **Contact Forms:** Set CAPTCHA functionality, required fields, validation, and verify information emailed or routed to CRM.
* [ ] **Newsletter Forms** Check signup forms functionality and verify user information pushed to third-party tool. 
* [ ] **Comments:** Set moderation notices be sent to appropriate email addresses. 
* [ ] **Search:** Verify CMS search or Google custom search traversing only necessary data, and returning correct results.
* [ ] **API Configuration:** Set live domain to be witelisted with third party intergrations or SaaS tools.
* [ ] **Dev Domains:** Verify database and assets not referencing dev, staging, or QA environments.
* [ ] **DNS:** Verify proper set up.
* [ ] **Conversions & Funnels:** Set analytics tools to collect visitor clickstream.
* [ ] **Payment System:** Turn off test mode off and transactions work. 
* [ ] **www / non-www:** Set non-canonical to redirect to canonical and preserving URL. 

—

## WordPress
### Best Practices
* [ ] **.htaccess:** Set with appropriate settings. 
* [ ] **Navigation** Set navigation and sub menus to always be accessible.
* [ ] **Pagination** Set next and previous links go to right content
* [ ] **Database Table Prefix:** Change from wp_. 
* [ ] **Plugins:** Remove unused plugins. 
* [ ] **Themes:** Remove unused themes. 
* [ ] **Version:** Remove generator meta in header. 
* [ ] **Admin Account:** Rename from admin.
* [ ] **Security Key:** Change from default. 
* [ ] **Admin URL:** Change from default. 