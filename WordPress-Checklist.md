# WordPress Checklist

## Setup

### Best Practices

* **Web Server Configuration** - Point to root WordPress folder. URL should not contain 'WordPress' anywhere.
* **Database Table Prefix** - Change from wp_. 
* **Database Connection** - Change to connect to dev database. 
* **Plugins** - Remove unused plugins. 
* **Themes** - Remove unused themes. 
* **Version** - Remove generator meta in header. 
* **Admin Account** - Rename from admin.
* **Security Keys & Salts** - Change from default. 
* **Admin URL** - Change from default. 
* **Default Content** - Remove default posts, comments, and pages.
* **Default Date / Time** - Set in Settings > General.
* **Default Blog Category** - Change from uncategorized.
* **Media Settings** - Set to month and year or appropriate file path.
* **Permalinks** - Set to post name or appropriate URL structure.
* **Site Title** - Set to proper website title.
* **Site Tag** - Set to proper website tagline.
* **Admin Email** - Update to someone on web development team. This is not the same as admin user account.
* **Memory Limit** - Set memory limit to maximum allowed by server or web host.
* **Auto Save** - Set number of seconds between auto-saves.
* **Multisite** - Enable if needed.
* **Debug Flag**- Enable during development.
* **Cache** - Disable during development.
* **Search Engine Visibility** - Disable development environment from being crawled by seach engines.
* **Sample Config File** - Remove wp-config-sample.php.
* **Version Control** - Set up repository to store and track files and changes.

---

## Theme Design

### Best Practices

* **Login Page** - Update with site brand.
* **Underlined Links** - Underline to help with usability and accessibility.
* **Visited vs Unvisited Link Colors** - Use different colors for usability.
* **Hover / Focus / Active Links** - Visually distingush when in hover, focus, or active states.
* **Color Contrast** - Contrast ratio should be minimum 4.5:1 for WCAG 2.0 AA compliance.
* **Form Placeholder Text** - Set placeholder attribute in input elements.
* **Descriptive Buttons** - Use pattern Verb Noun, like Upload File, instead of Ok or Submit.


------

## Coding

### Best Practices

- **Core Files** - Never modify any WordPress core files.
- **Database Queries** - Don't use `mysqli_query()`, instead use `$wpdb` object or `WP_Query`.
- **'DISTINCT', 'GROUPBY'** - Avoid cross-table queries and any other operations which create temporary tables.
- **Query Result Limits** - Add maximum number of results returned to prevent killing database.
- **Indexes** - Verify indexes are used in queries by running `EXPLAIN` statement.
- **Address Bar** - Only show encrypted session values in address bar.

### Plugins

- **Mail** - Use `wp_mail()` instead of PHP `mail()` function.
- **Clean Inputs / Outputs** - Sanitize/escape all inputs and outputs to prevent Cross-Site Scripting (XSS) problems.
- **Nonces** - Protect against Cross-Site Request Forgery (CSRF) when expecting user submitted data.
- **Data Validation** - Use JavaScript, built-in PHP functions, core WordPress functions, and/or custom functions to validate inputs before processing.
- **Cache DOM Queries** - Cache jQuery selectors for re-use on page.
- **Event Delegation** - Reduce individual element event handling by using event delegation instead.
- **Deactivate / Uninstall Hooks** - Implement to cleanup data.
- **Prefix** - Add plugin name abbreviation as prefix to variables, functions, and classes.
- **Folder Structure** - Separate into includes, admin, and public folders.
- **Roles and Rights** - Verify authentication and authorization of user when plugin called.
- **Settings / Options API** - Use to build admin pages.

### Themes

- **Child Themes** - Create child theme if modifiying existing theme allows for child themes and changes are not extensive.
- **File Structure** - Separate into include, asset, and template parts folders. 
- **Template Tags** - Instead of hardcoding, use template tags and conditional tags as much as possible.
- **Enqueue Stylesheets** - Use `wp_enqueue_style` and template tags for directory paths instead of hardcoding links to CSS files.
- **Enqueue JavaScript** - Use `wp_enqueue_scripts` and template tags for directory paths instead of hardcoding links to JavaScript files.
- **File Naming** - Use standard WordPress naming hierarchy. 
- **Theme Unit Test** - Use WordPress Theme Unit Test to visually inspect and test theme and test using Theme Check plugin even though theme will not be submitted to WordPress theme directory.
- **Screenshot** - Create screenshot with look and feel of theme.
- **Jetpack Infinite Scroll** - Support if needed.
- **'$content_width'** - Set.


## Theme HTML

### Best Practices
* **HTML5 Semantic Elements** -  Use HTML5 semantic elements appropriately.
* **Error pages** -  Create 404 page and 5xx error pages. 5xx error pages can be handled by web server.
* **AMP / Instant Articles** - Generate stripped down HTML for Google and Facebook.
* **Labels / Inputs** - Connect labels to inputs using `for` attribute in labels.

### Head
* **Doctype** - Set Doctype to HTML5 and put at the top of header.
* **Charset** - Set to UTF-8.
* **X-UA-Compatible** -  Set for backwards IE compatibility.
* **Viewport** -  Set viewport.
* **Favicons** -  Set favicon file location.
* **Apple Touch & Android Icons** -  Set Apple touch & Android icons.
* **Canonical** -  Set ``rel=“canonical”``.
* **Language tag** -  Set language tag.
* **Conditional comments** -  Set conditional comments for IE.
* **RSS feed** -  Set RSS URL or remove.
* **Smart App Banner** - Set app-id and app-argument if app available from app store.
* **Facebook Open Graph** - Set and link to images.
* **Twitter Card** - Set and link to images.

### HTML Testing
* **W3C Compliance** -  Run pages through W3C validation tools.
* **Desktop Browsers** -  Test pages on current (and back one version) of current desktop browsers.
* **Mobile Browsers** -   Test pages on current (and back on version) current mobile browsers.
* **Link Checker** -  Run pages through broken link checkers.
* **Adblockers Test** -  Verify adblockers do not break pages.

___

## Theme Fonts
### Best Practices
* **Webfont Formats** -  Convert fonts to WOFF, WOFF2 and TTF file formats.
* **Fall-back Typefaces** -  List 2 or more in case desired fonts not available.
* **Service Configuration** - Set live domain and development IPs to be white-listed with hosted font services.

___

## Theme CSS
### Best Practices
* **Preprocessors** -  Remove links to intermediary preprocessor files. 
* **Breakpoints** - Check content, flow, and UX work as intended at different breakpoints.
* **CSS Print** -  Set print stylesheet for each page.
* **Unique ID** -  Use unique IDs per page.
* **Reset CSS** - Use CSS reset stylesheet.
* **JavaScript Prefix** -  Name classes or IDs with **js-** when modified by JavaScript and not by CSS files.
* **Inline / Embedded CSS** -  Remove or minimize embedded or inline CSS.
* **Vendor Prefixes** -  Use CSS vendor prefixes depending on required browser support compatibility.
* **Stylesheet Layout** - Order of properties display > positioning > box model > colors and typography > other.
* **Media Queries** - Place at bottom of stylesheet.
* **Magic Numbers** - Avoid.
* **Main Stylesheet Header** - Include theme name, author, description, version, license, license URI, and text domain.
* **Sticky Posts** - Set to be visually distinguishable. 

### Performance
* **Concatenation** -  Concatenate CSS files.
* **Minification** -  Minify CSS files.
* **Non-blocking** -  Verify CSS files are non-blocking in theme template.
* **Unused CSS** -  Cleanup CSS.

### CSS Testing
* **CSS Validator** - Run stylesheets through CSS validators.

___

## Theme Images / Videos
### Best Practices
* **Placeholder Images** - Replace with real images.
* **Stock Images** - Replace stock watermarked images replaced with licensed versions. 
* **Optimization** -  Optimize for needed browsers and devices.
* **Retina** -  Use x2 or 3x images to support retina display.
* **Width and Height** -  Set ``<img>`` to have height and width, handle with CSS and media queries, or serve appropriate sizes for respective browsers and devices.
* **Alternative text** -  All ``<img>`` have an alternative text which describe the image visually.
* **Lazy loading** -  Load images on scroll or as needed.
* **Social Thumbnails**: Generate Facebook/Twitter/LinkedIn thumbnails for all pages.
* **Responsive Video Players** -  Videos resize appropriately on different browsers and devices.
* **Video Controls** - Show playblack, pause, and mute controls.
* **Logo** - Set logo link to return visitor to homepage.

------

## Theme JavaScript

### Best Practices
* **jQuery Version**- Do not add newer jQuery libraries if available.
* **'$' Shortcut** - Use IIFE to create.
* **JavaScript Inline** -  Remove or minimize inline JavaScript.
* **Concatenation** -   Concatenate Javascript files.
* **Minification** - Minify JavaScript files.
* **Non-blocking** -  Load JavaScript files asynchronously.
* **Modernizr** -  Use Modernizr or similar tool to test for specific browser features.
* **Footer Load** - Place scripts in footer of page.
* **eval()** - Never, ever use.

### JavaScript testing
* **ESLint** - Verify JavaScript with ESLint or similar tool.

___

## Copy

### Best Practices

- **Text** - Replace all Lorem Ipsum with real copy.

------

## Security

### Best Practices
* **HTTPS** - Use HTTPS.
* **HSTS** - Set HTTP Strict Transport Security parameter on web server.
* **Password Reset** - Set password rules and flow on all authentication pages like Registration, forgot password, change password.
* **Login Limits** - Require ‘human’ verification after a defined number of failed tries.
* **System Information** - Verify application, server, or database version or connection information not publicly viewable.
* **SSL** - Verify certificate not expiring. 
* **Exploit Scanner** - Run plugin on site.

___

## Performance
### Best practices
* **Minified** - Minimize HTML and enable gzip type compression on web server.
* **Lazy loading** - Load images, scripts, and CSS files as needed, not on load.
* **Cookie size** - Minimize size of cookies.
* **Content Delivery Network** - Push CSS, JavaScript, fonts, and generated HTML to CDN.
* **HTTP Cache Headers** - Set approriate parameters.
* **DNS Prefetching** - Enable ``preload`` and/or ``dns-prefetch``.
* **Mixed Content** - Retrieve all files and assets via HTTPS.
* **Logging** - Enabled tools and verify data passing to monitoring platforms.

___

## SEO
### Best Practices
* **Tag Manager** - Set up and verify data passing to tools.
* **Analytics & Conversion** -  Google Analytics and similar tools installed,correctly configured, and registering data. 
* **Exclude IPs** - Remove office or home IPs from analytics and conversion tools.
* **Ad Pixels** - Verify all ad pixels installed and registering.
* **Heatmaps**: Verify installation, configuration, and data flow to third party tools.
* **A/B Tests**: Verify installation, configuration, and data flow to third party tools.
* **Chat** - Verify installation, configuration, and data flow to third party tool.
* **Sitemap XML** - Install plugin to auto-generate and submit of site, image, and video XMLs to Google Webmaster Tools and similar tools
* **Google Webmaster Tools** - Verify no errors noted by WMT or similar tools.
* **robots.txt** - Verify robots.txt not blocking any pages.
* **Structured Data or Rich Snippets** -  Generate error-free structured data as needed.
* **Title** -  Use unique title tag used on each page.
* **Description** -  Set unique meta description on each page.
* **301 Redirects** - Return 301 for moved content
* **Redirections** - Use Rewrite Rules Inspector plugin and check redirections.
* **Title Attribute** - Set ``title`` attribute for all links.
* **Social Widgets** - Connect social accounts and set up to show buttons / links in right places.

___

## Legal
### Best Practices
* **Privacy Policy** -  Create page and put link in footer.
* **Terms of Service** -  Create page and put link in footer.
* **GDPR Compliance** - Show consent notice visible.
* **Copyright** - Show in footer. 

___

## Pre-Launch
### Best Practices
* **.htaccess** - Set with appropriate settings. 
* **Backups** - Check backup and restore systems functional. Fully backup old site if one exists.
* **Versioning** - Branch or tag production code in version control system.
* **Contact Forms** - Set CAPTCHA functionality, required fields, validation, and verify information emailed or routed to CRM.
* **Newsletter Forms** Check signup forms functionality and verify user information pushed to third-party tool. 
* **Comments** - Set moderation notices be sent to appropriate email addresses. 
* **Search** - Verify WordPress search or Google custom search traversing only necessary data, and returning correct results.
* **API Configuration** - Set live domain to be witelisted with third party intergrations or SaaS tools.
* **Dev Domains** - Verify database and assets not referencing dev, staging, or QA environments.
* **DNS** - Verify proper set up.
* **Conversions & Funnels** - Set analytics tools to collect visitor clickstream.
* **Payment System** - Turn off test mode off and transactions work. 
* **www / non-www** - Set non-canonical to redirect to canonical and preserving URL. 
* **Debug Mode** - Disable in wp_config.php. 
* **WordPress Address (URL)** - Update to production URL in wp-config.php or Settings > General
* **Site Address (URL)** - Update to production URL in wp-config.php or Settings > General
* **Plugin / Theme Auto-Updates** - Update usernames, passwords, and API keys.
* **Gravatars** - Set up user accounts with Gravatars if necessary.
* **Pagination** - Verify 'next' and 'previous' display right content in respective categories.
* **Folder and File Permissions** - Verify folder contents are not viewable and individual PHP files cannot be downloaded. 
* **Upload Permissions** - Verify images and attachments can be uploaded via backend and downloaded by non-logged in users. 
* **Spam Protection** - Enable Akismet plugin and delete old spam comments.
* **Post Revisions** - Limit number of post revisions saved and delete post revisions generated during development.
* **Trash** - Set number of days when deleted content can be removed from database.
* **Cache** - Enable default WordPress caching or a third-party plugin.
* **Admin Email** - Set to individual responsible for website post-launch.
- **Search Engine Visibility** - Enable search engines to index site.

------

## Post-Launch

### Best Practices

- **Update Files** - Set auto-update for core, themes, and plugins or create monthly or quarterly plan to test and roll out updates, especially if custom functionality was built for the website. 
- **Documentation** - Compile website, webhost, S/FTP, and social logins, along with expiration dates on third-party services, SSL, stock photography, etc, and share with appropriate individuals.
- **Error Logs** - Check web server logs for PHP errors on a regularly scheduled basis. 
- **Version Control** - Transfer ownership of repository to client if necessary.