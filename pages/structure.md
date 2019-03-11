---
title: Starter Theme
description: This a basic theme that helps you get your interface up and running quickly. It provides all required theme templates, starter set of liquid tags, and some basic styles and modules for you to extend on.
---

Liquid objects contain attributes to output dynamic content on the page.
For example, the product object contains an attribute called title that can be used to output the title of a product.

**Liquid objects** are also often referred to as **Liquid variables**.

To output an object's attribute, wrap the object's name in **{{** and **}}**, as shown below:


<p class="code-label">Input</p>
```liquid
{% raw %}
├── assets
│   └── Javascript, CSS, and theme images
├── layout
│   ├── mailer.liquid
│   ├── theme.liquid
│   └── optional alternate layouts
├── snippets
│   └── custom code snippets
├── templates
│   ├── 404.liquid
│   ├── cart.liquid
│   ├── checkout.reserved.liquid
│   ├── checkout.expired.liquid
│   ├── checkout.store.liquid
│   ├── checkout.subscription.liquid
│   ├── checkout.event.liquid
│   ├── checkout.season.liquid
│   ├── collection.liquid
│   ├── collection.list.liquid
│   ├── credential.season.liquid
│   ├── credential.subscription.liquid
│   ├── directory.events.liquid
│   ├── directory.liquid
│   ├── event.liquid
│   ├── index.liquid
│   ├── inscription.liquid
│   ├── list-collections.liquid
│   ├── order.event.liquid
│   ├── order.inscription.liquid
│   ├── order.season.liquid
│   ├── order.store.liquid
│   ├── order.subscription.liquid
│   ├── orders.liquid
│   ├── page.contact.liquid
│   ├── page.liquid
│   ├── product.liquid
│   ├── search.liquid
│   ├── season.liquid
│   ├── store.liquid
│   ├── subscription.detail.liquid
│   ├── subscription.new.liquid
│   ├── customers
│   │     ├── account.liquid
│   │     ├── active_account.liquid
│   │     ├── forgot_password.liquid
│   │     ├── login.liquid
│   │     ├── register.liquid
│   │     ├── reset_password.liquid
│   │     ├── start.liquid
│   │     ├── orders.liquid
│   │     └── required templates if customer accounts are enabled
│   └── mailers
│         ├── customer.confirmation_instructions.liquid
│         ├── customer.magic_link_instructions.liquid
│         ├── customer.password_change.liquid
│         ├── customer.reset_password_instructions.liquid
│         ├── customer.unlock_instructions.liquid
│         ├── customer.final_warning.liquid
│         ├── customer.order.coupon.liquid
│         ├── order.event.liquid
│         ├── order.inscription.liquid
│         ├── order.liquid
│         ├── order.season.liquid
│         ├── order.season.reminder_of_instalments.liquid
│         ├── order.store.liquid
│         ├── subscription.cancelling.liquid
│         ├── subscription.cancelled.liquid
│         ├── subscription.failed.liquid
│         ├── subscription.new.liquid
│         └── subscription.successful.liquid
{% endraw %}
```
### Detailed description

#### Assets

The `assets` directory is rendered as the **Assets** folder in the theme editor. It contains all the assets used in the theme, including images, stylesheets, and javascript.

#### Configs

*Currently unused*

The `config` directory is rendered as the **Configs** folder in the theme editor. It includes a `settings_schema.json` file and a `settings_data.json` file

#### Layouts

The `layout` directory is rendered as the Layouts folder in the theme editor. It contains theme layout templates, which by default is the `theme.liquid` file. All Liquid templates inside the templates folder are rendered inside the `theme.liquid` file.

#### Locales

The `locales` directory is rendered as the Locales folder in the theme editor. It contains the theme's locale files, which are used to provide translated content for the theme.

Among other files, this folder contains the default Spanish locale file, `es.default.json` (that also defines the default language).

#### Sections

The `sections` directory is rendered as the **Sections** folder in the theme editor. It contains a theme's sections, which are reusable modules of content that can be customized and re-ordered by users of the theme.

#### Snippets

The `snippets` directory is rendered as the **Snippets** folder in the theme editor. It contains all the theme's Liquid snippet files, which are bits of code that can be referenced in other templates of a theme.

Use the Liquid `include` tag to load a snippet into your theme.
