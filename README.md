# Hydrogen Redirect Theme

[Download](https://github.com/Shopify/hydrogen-redirect-theme/archive/refs/heads/master.zip)

When launching a Hydrogen storefront, you’ll likely also want to redirect
any traffic that happens to hit your Liquid store too. This theme allows you
helps you do that while also making sure you retain features like the bot
detection checkpoint, and discount links.

## Setup

1. [Download the theme](https://github.com/Shopify/hydrogen-redirect-theme/archive/refs/heads/master.zip)
2. Navigate to **Online Store -> Themes** in your Shopify admin
3. **Upload** the theme to your Theme Library
4. **Customize** the Redirect theme
5. Go to **Theme settings -> Storefront** and configure `storefront_hostname`
6. **Publish** the theme

## Gift cards

Since the Shopify Storefront API does not yet support fetching gift cards, a customizable `gift_card.liquid` template has been added.

## Checkpoint template for Bot Protection

See: https://shopify.dev/docs/custom-storefronts/oxygen/migrate/redirect-traffic#enabling-bot-protection-for-flash-sales

### Credit

This was based on a theme from Instant Commerce, which you can [find here](https://github.com/instantcommerce/shopify-headless-theme).
