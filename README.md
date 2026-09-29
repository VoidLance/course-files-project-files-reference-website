# Elegant Yachting Tours

Elegant Yachting Tours is a responsive, multi-page website for presenting luxury yacht experiences. Visitors can browse available tours, view tour details and photography, learn about the company, and send a message through the contact form.

## Features

- Landing page with a yacht hero image and calls to action
- Tour catalogue with pages for:
  - Island Hopping Adventure
  - Sunset Cruise
  - Underwater Exploration
- Responsive photo gallery backed by local images in [`images/`](images/)
- About page describing the service
- Contact form with basic server-side validation and email delivery
- Responsive styling in a single custom stylesheet

## Technology

- HTML5
- CSS3
- Vanilla JavaScript
- PHP for contact-form handling
- Google Fonts and Font Awesome loaded from their hosted CDNs

There is no package manager, build step, or compiled output. The site is served directly from the project files.

## Getting started

### Requirements

- A modern web browser
- PHP 7+ for the contact form and local development server
- A mail transport configured for PHP's `mail()` function if contact messages should be delivered

### Run locally

From the repository root, start PHP's built-in server:

```bash
php -S localhost:8000
```

Open [http://localhost:8000/home.html](http://localhost:8000/home.html) in a browser. The navigation links connect the site pages:

- [`home.html`](home.html) — homepage
- [`tours.html`](tours.html) — tour catalogue
- [`tour1.html`](tour1.html), [`tour2.html`](tour2.html), [`tour3.html`](tour3.html) — tour details
- [`gallery.html`](gallery.html) — image gallery
- [`about.html`](about.html) — company overview
- [`contact.html`](contact.html) — contact form

To test the contact form, configure a working PHP mail transport and review the recipient address in [`form-handler.php`](form-handler.php) before submitting the form.

### Deploy

Copy the project files to any web host that serves HTML, CSS, images, and PHP. Keep the relative paths and the `images/` directory intact. A PHP-capable host is required for [`form-handler.php`](form-handler.php); the informational pages can also be served by a static web server.

## Project structure

```text
.
├── home.html
├── tours.html
├── tour1.html
├── tour2.html
├── tour3.html
├── gallery.html
├── about.html
├── contact.html
├── form-handler.php
├── style.css
└── images/
```

## Support

For questions about the site, use the contact details or social links presented in the website footer. For a local development issue, first confirm that the PHP server is running from the repository root and that the required asset paths are available.

## Contributing

Contributions are welcome. Before opening a change:

1. Fork the repository and create a focused branch.
2. Make the smallest change that addresses the issue or improvement.
3. Check the affected pages in a browser at common desktop and mobile widths.
4. Verify that navigation, local images, and the contact form still work.
5. Submit a pull request describing the change and how it was tested.

Please keep the existing plain HTML/CSS/JavaScript/PHP approach unless a change requires otherwise. Follow any licensing terms shown on the repository's GitHub page.

## Maintainer

The project is authored and maintained by Alistair Sweeting. See the repository's GitHub page for current maintainer and contribution activity.
