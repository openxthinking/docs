# How to

## Upload files

1. From `Shopify admin`, go to `Settings → Files`
1. Click <kbd>Upload files</kbd>
1. Select up to 20 files to upload, and then click <kbd>Open</kbd>
1. Copy the file URL from `Link` button

![Upload files](https://docs.openthinking.net/media/global/howto/upload-files.png "Upload files")

`Max file size: 20MB`


[Learn more](https://help.shopify.com/en/manual/shopify-admin/productivity-tools/file-uploads) about file uploads.


## Custom code

1. From `Shopify admin`, go to `Online Store → Themes`
1. Click <kbd>Customize</kbd>
1. Open `Theme settings`, and scroll to `Custom code`
1. In the `CSS or JS` section paste your code
1. <kbd>Save</kbd>

![Customize](https://docs.openthinking.net/media/global/howto/online_store-themes-customize.png "Customize")
![Custom CSS](https://docs.openthinking.net/media/global/howto/theme_settings-custom_code.png "Custom CSS")


## Create or edit files

?> Before you customize your theme, it’s best practice to duplicate your theme to create a backup copy. This makes it easy to discard your changes and start again if you need to. [Learn how](https://bullet.docs.openthinking.net/#/customization?id=backup)


#### Edit file

1. From `Shopify admin`, go to `Actions → Edit code`
1. In the `search bar` type the name of the file you're looking for
1. Click to <kbd>Open</kbd> the file
1. <kbd>Save</kbd>

![Edit code](https://docs.openthinking.net/media/global/howto/edit_code.png "Edit code")
![Code editor](https://docs.openthinking.net/media/global/howto/edit_code-code_editor.png "Code editor")

#### Create file

1. From `Shopify admin`, go to `Actions → Edit code`
1. Open the directory you need to create the file in (e.g. Sections)
1. Click the <kbd>Add new ****</kbd> link (e.g. Add new Section)
1. Remove the auto-generated boilerplate code
1. Paste your code
1. <kbd>Save</kbd>

![Edit code](https://docs.openthinking.net/media/global/howto/edit_code.png "Edit code")
![Edit code](https://docs.openthinking.net/media/global/howto/edit_code-the_editor.png "Edit code")



## Templates
Templates control what's rendered on each type of page in a theme. You can create multiple versions of the same template type to create custom templates for different use cases. For example, you can create a separate product template for outerwear products or a separate page template for pages with video content.

#### Create template
1. From Shopify admin, go to `Online Store → Themes`
1. Click <kbd>Customize</kbd>
1. In the "Home page" dropdown, select `Pages`
1. Click <kbd>[+] Create template</kbd>
1. Enter the name for your template
1. Select the template you want your new template to be based on
1. Click <kbd>Create template</kbd>

![Edit code](https://docs.openthinking.net/media/global/howto/templates_steps.png)

#### Assign template
1. From the left bar click <kbd>Change</kbd>
1. Select the page you want to assign the new template to
1. <kbd>Save</kbd>

![Edit code](https://docs.openthinking.net/media/global/howto/templates_customize_template.png)

#### Assign template v2
In case the first option to assign the page doesn't work, use this instead.

1. From Shopify admin, go to `Online Store → Pages`
1. Open the page, in `Online store` block, and assign a template from your current theme to define how the page is displayed.
1. <kbd>Save</kbd>

![Edit code](https://docs.openthinking.net/media/global/howto/templates_select_template.png)

### Access unpublished template
Shopify limits the templates in the admin to those included in your published theme. Often times you'll require access to templates in an unpublished theme but you are not ready to publish the new theme to unlock them. To address this, we suggest completing this workaround.

!> Before continuing with this guide, make sure you have purchased the theme.

Step 1:
1. From `Shopify admin`, go to `Online store → Themes`
1. Locate **Bullet**, select `Actions → Edit code`
1. Under `Templates`, locate the name of the template you're going to make accessible (e.g. `page.about.json`)
1. No changes are needed here — we just need the name confirmed for the next step

Step 2: 
1. From `Shopify admin`, go to `Online store → Themes`
1. Click <kbd>Actions</kbd> then <kbd>Edit code</kbd> beside your published theme (e.g. Dawn)
1. Under `Templates`, select <kbd>(+) Add a new template</kbd>
1. For **"Create a new template for"**, select the base template (for this example, **page**)
1. For the **File name**, add the custom template's name (for this example **about**). ⚠️ This needs to match the spelling of the unpublished theme's template name.
![Edit code](https://docs.openthinking.net/media/global/howto/unpublished_templates.png)
1. Click <kbd>Create template</kbd>
1. Open the default Template file for the template type (e.g. `page.json`)
1. Copy the code from the default file to replace the new file
1. <kbd>Save</kbd>

Step 3: Confirm the template is accessible
1. From `Shopify admin`, go to `Online store → Pages`
1. Open the page you want (e.g. **About us**)
1. On the right side, in the **"Theme template"** select dropdown
1. Click and select **"about"**
![Edit code](https://docs.openthinking.net/media/global/howto/unpublished_templates_theme_template.png)
1. <kbd>Save</kbd>


## Preview link

1. From `Shopify admin`, go to `Online store → Themes`
1. Locate the theme, then click <kbd>Actions</kbd> → `Preview`
1. Click <kbd>Share preview</kbd> at the bottom of the page that just opened
1. Click <kbd>Copy link</kbd>

![Edit code](https://docs.openthinking.net/media/global/howto/preview-actions-preview.png)
![Edit code](https://docs.openthinking.net/media/global/howto/preview-share_link.png)
![Edit code](https://docs.openthinking.net/media/global/howto/preview-copy_link.png)

!> The preview link is available for a few days. After that, you need to generate a new one.


## Metafields

Use OpenThinking themes in combination with the new Metafields to provide dynamic content in page blocks.


#### Step 1: Add new metafield definition

1. From `Shopify admin`, open `Settings`
1. Click <kbd>Metafields</kbd>, and open `Products`
1. Select <kbd>Add definition</kbd>
1. <kbd>Save</kbd>

![Add metafield](https://docs.openthinking.net/media/global/howto/metafields-add.png "Add metafield")
![Add definition](https://docs.openthinking.net/media/global/howto/metafields-add_definition.png "Add definition")
![Add definition](https://docs.openthinking.net/media/global/howto/metafields-add_definition_example.png "Add definition")

#### Step 2: Fill metafield in products

1. From `Shopify admin`, click <kbd>Products</kbd>
1. Open a product
1. Scroll down to `Metafields`
1. Enter the data value to the new metafield
1. <kbd>Save</kbd>

![Edit value](https://docs.openthinking.net/media/global/howto/metafields-product-add_value.png "Edit value")


#### Step 3: Display metafield on product page

1. From `Shopify admin`, go to `Online Store → Themes`
1. Click <kbd>Customize</kbd>, then open a product template
1. Select <kbd>(+) Add block</kbd>, then `Text`
1. In the top-right corner of the sidebar, select `Insert dynamic source`

![Dynamic source](https://docs.openthinking.net/media/global/howto/metafields-insert_dynamic_source.png "Dynamic source")

---

#### Not supported metafields

?> Not all metafield types are available with the available blocks. For example, if you need to display an image you'll need to use the `Custom Liquid` block, instead, and call the metafield with Liquid code.

1. From `Shopify admin`, go to `Online Store → Themes`
1. Click <kbd>Customize</kbd>, then open a product template
1. Select <kbd>(+) Add block</kbd>, then `Custom Liquid`
1. Get your metafield values with Liquid

Generates a text version of the metafield data.

```liquid
{{ product.metafields.openthinking.instructions_wash | metafield_text }}
```

code above returns:
```html
This is a single line of text.
```

---

Generates an HTML element depending on the type of metafield.

```liquid
{{ product.metafields.openthinking.instructions_wash | metafield_tag }}
```

code above returns:
```html
<span class="metafield-single_line_text_field">This is a single line of text.</span>
```


##### External links 
- [Metafields](https://help.shopify.com/en/manual/metafields)
- [Metafields API](https://shopify.dev/api/liquid/objects/metafield)
- [Metafield filters](https://shopify.dev/api/liquid/filters/metafield-filters)
- [Metafield compatibility](https://shopify.dev/themes/architecture/settings#dynamic-sources)


## Change payments icons

The payment icons that show in your theme's footer are determined by your store's [payment settings](https://help.shopify.com/en/manual/payments) and the customer's region and currency. You can disable payment icons in the theme editor in the footer section. If you want to add or remove payment icons without changing your payment settings, then you can do so by editing your theme code.

1. From your Shopify admin, go to `Online Store > Themes`.
1. Find the theme you want to edit, and then click <kbd>Actions</kbd> and <kbd>Edit code</kbd>.
1. In the Sections directory, click `footer.liquid`.
1. Find the following code in the file:

```liquid
{%- for type in shop.enabled_payment_types -%}
```

Replace it with:

```liquid
{%- assign enabled_payment_types = 'visa,master,apple_pay,paypal' | remove: ' ' | split: ',' -%}
{%- for type in enabled_payment_types -%}
```

In the code that you just pasted, there is a list of payment providers separated by commas: `visa,master,apple_pay,paypal`. The payment providers that you include in this list will determine which payment icons display on your online store. You can edit the list of payment providers to suit your needs.

<details>
	<summary>The values that you can use are listed below:</summary>

- `afterpay`
- `american_express`
- `apple_pay`
- `bitcoin`
- `dankort`
- `diners_club`
- `discover`
- `dogecoin`
- `dwolla`
- `facebook_pay`
- `forbrugsforeningen`
- `google_pay`
- `ideal`
- `jcb`
- `klarna`
- `klarna`
- `pay`
- `later`
- `litecoin`
- `maestro`
- `master`
- `paypal`
- `shopify_pay`
- `sofort`
- `visa`

</details>