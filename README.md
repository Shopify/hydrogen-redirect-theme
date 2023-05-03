# A Theme for Headless

Liquid theme that automatically redirects customers to your custom storefront.
[Download theme](https://github.com/benjaminsehl/shopify-headless-theme/archive/refs/heads/master.zip)

---

## Overview

When using a headless Shopify setup, you normally don't want customers to access any of the theme pages except the checkout. However, you can't totally disable the theme and a lot of links will still point to the theme (e.g. links in emails, plugins and the checkout).

The sole purpose of this Liquid theme is to automatically redirect customers that land on one of the theme pages to the related page in your custom storefront.

## Installation

1. Download the [shopify-headless-theme-master.zip](https://github.com/benjaminsehl/shopify-headless-theme/archive/refs/heads/master.zip) file
2. Navigate to **Online Store > Themes** in your Shopify admin
3. Upload the theme to your **Theme Library**
4. Click the **Customize** button of the newly installed theme
5. Configure the `storefront_hostname` in **Theme settings > Storefront**
6. **Publish** the theme 🚀

## Custom redirects

You can configure the `custom_redirects` value in **Theme settings > Storefront**.

The redirect rule format is as following:

```
Shopify path > Storefront path
```

Each line in the textarea represents a single redirect rule.

### Example configuration

The example below removes the `/account` prefix from the login, register and reset password redirects.

```
/account/login > /login
/account/register > /register
/account/reset > /reset-password
/account/activate > /activate-account
```

## Gift cards

Since the Shopify Storefront API unfortunately does not support fetching gift cards yet, a customizable `gift_card.liquid` template has been added.

### Credit
This was based on a theme from a similar theme from Instant Commerce, which you can [find here](https://github.com/instantcommerce/shopify-headless-theme), and merges in some previous work I'd published as [a gist here](https://gist.github.com/benjaminsehl/cdd0ce53951659db1266276cda854285).
