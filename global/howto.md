# How to

## Upload files

1. From `Shopify admin`, go to `Settings → Files`
1. Click `Upload files`
1. Select up to 20 files to upload, and then click `Open`
1. Copy the file URL from `Link` button

![Upload files](https://docs.openthinking.net/media/global/howto/upload-files.png "Upload files")

[Learn more](https://help.shopify.com/en/manual/shopify-admin/productivity-tools/file-uploads) about file uploads.


## Custom Code

1. From `Shopify admin`, go to `Online Store → Themes`
1. Click `Customize`
1. Open `Theme settings`, and scroll to `Custom code`
1. In the `CSS or JS` section paste your code
1. `Save`

![Customize](https://docs.openthinking.net/media/global/howto/online_store-themes-customize.png "Customize")
![Custom CSS](https://docs.openthinking.net/media/global/howto/theme_settings-custom_code.png "Custom CSS")

## Metafields

Use OpenThinking themes in combination with the new Metafields to provide dynamic content in page blocks.


#### Step 1: Add new metafield definition

1. From `Shopify admin`, open `Settings`
1. Click `Metafields`, and open `Products`
1. Select `Add definition`
1. `Save`

![Add metafield](https://docs.openthinking.net/media/global/howto/metafields-add.png "Add metafield")
![Add definition](https://docs.openthinking.net/media/global/howto/metafields-add_definition.png "Add definition")
![Add definition](https://docs.openthinking.net/media/global/howto/metafields-add_definition_example.png "Add definition")

#### Step 2: Fill metafield in Products

1. From `Shopify admin`, click `Products`
1. Open a product
1. Scroll down to `Metafields`
1. Enter the data value to the new metafield
1. `Save`

![Edit value](https://docs.openthinking.net/media/global/howto/metafields-product-add_value.png "Edit value")


#### Step 3: Display metafield on Product page

1. From `Shopify admin`, go to `Online Store → Themes`
1. Click `Customize`, then open a product template
1. Select `(+) Add block`, then `Text`
1. In the top-right corner of the sidebar, select `Insert dynamic source`

![Dynamic source](https://docs.openthinking.net/media/global/howto/metafields-insert_dynamic_source.png "Dynamic source")

---

#### Display not supported metafields

?> Not all metafield types are available with the available blocks. For example, if you need to display an image you'll need to use the `Custom Liquid` block, instead, and call the metafield with Liquid code.

1. From `Shopify admin`, go to `Online Store → Themes`
1. Click `Customize`, then open a product template
1. Select `(+) Add block`, then `Custom Liquid`
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