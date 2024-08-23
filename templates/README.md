# Templates
This directory contains the base HTML templates used across the MusicHUB application.

## Structure
```bash
templates/
├── base.html # Base template for the application
├── layout.html # Layout template for the application
├── navbar.html # Navbar template for the application
└── footer.html # Footer template for the application
```

## Files

- **base.html**: The base template that includes the common structure for all pages.
- **layout.html**: The layout template that defines the main layout of the application.
- **navbar.html**: The template for the navigation bar.
- **footer.html**: The template for the footer.

## Usage

To use these templates, extend them in your specific HTML files. For example, to use the `base.html` template:

```html
{% extends "base.html" %}

{% block content %}
<h1>Welcome to MusicHUB</h1>
{% endblock %}
```

These templates help maintain a consistent look and feel across the application.