# How to

## Upload files

1. From `Shopify admin`, go to `Settings → Files`
1. Click <kbd>Upload files</kbd>
1. Select up to 20 files to upload, and then click <kbd>Open</kbd>
1. Copy the file URL from `Link` button

![Upload files](https://docs.openthinking.net/media/global/howto/upload-files.png "Upload files")

`Max file size: 20MB`


[Learn more](https://help.shopify.com/en/manual/shopify-admin/productivity-tools/file-uploads) about file uploads.


## Custom Code

1. From `Shopify admin`, go to `Online Store → Themes`
1. Click <kbd>Customize</kbd>
1. Open `Theme settings`, and scroll to `Custom code`
1. In the `CSS or JS` section paste your code
1. <kbd>Save</kbd>

![Customize](https://docs.openthinking.net/media/global/howto/online_store-themes-customize.png "Customize")
![Custom CSS](https://docs.openthinking.net/media/global/howto/theme_settings-custom_code.png "Custom CSS")


## Create, Edit files

?> Before you customize your theme, it’s best practice to duplicate your theme to create a backup copy. This makes it easy to discard your changes and start again if you need to. [Learn how](https://bullet.docs.openthinking.net/#/customization?id=backup)


#### Edit file

1. From `Shopify admin`, go to `Actions → Edit code`
1. In the `search bar` type the name of the file your're looking for
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
Templates control what's rendered on each type of page in a theme. You can create multiple versions of the same template type to create custom templates for different use cases. For example, you can create a separate product template for outerwear products, or a separate page template for pages with video content.

#### Create template
1. From Shopify admin, go to `Online Store → Themes`
1. Click <kbd>Customize</kbd>
1. In the "Home page" dropdown, select `Pages`
1. Click <kbd>[+] Create template</kbd>
1. Enter the name for your template
1. Select the template you want your new template to be based on
1. Click <kbd>Create template</kbd>

![Edit code](https://docs.openthinking.net/media/global/howto/templates_steps.png)

#### Assign to page
1. From the left bar click <kbd>Change</kbd>
1. Select the page you want to assign the new template to
1. <kbd>Save</kbd>

![Edit code](https://docs.openthinking.net/media/global/howto/templates_customize_template.png)

#### Assign to page option 2 
In case the first option to assign the page doesn't work, use this instead.

1. From Shopify admin, go to `Online Store → Pages`
1. Open the page, in `Online store` block, assign a template from your current theme to define how the page is displayed.
1. <kbd>Save</kbd>

![Edit code](https://docs.openthinking.net/media/global/howto/templates_select_template.png)



## Generate preview link

1. From `Shopify admin`, go to `Online store → Themes`
1. Locate the theme, then click <kbd>Actions → Preview</kbd> 
1. Click <kbd>Share preview</kbd> at the bottom of the page that just opened
1. Click <kbd>Copy link</kbd>

![Edit code](https://docs.openthinking.net/media/global/howto/preview-actions-preview.png)
![Edit code](https://docs.openthinking.net/media/global/howto/preview-share_link.png)
![Edit code](https://docs.openthinking.net/media/global/howto/preview-copy_link.png)

!> The preview link is available for few days. After that you need to generate a new one.


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

#### Step 2: Fill metafield in Products

1. From `Shopify admin`, click <kbd>Products</kbd>
1. Open a product
1. Scroll down to `Metafields`
1. Enter the data value to the new metafield
1. <kbd>Save</kbd>

![Edit value](https://docs.openthinking.net/media/global/howto/metafields-product-add_value.png "Edit value")


#### Step 3: Display metafield on Product page

1. From `Shopify admin`, go to `Online Store → Themes`
1. Click <kbd>Customize</kbd>, then open a product template
1. Select <kbd>(+) Add block</kbd>, then `Text`
1. In the top-right corner of the sidebar, select `Insert dynamic source`

![Dynamic source](https://docs.openthinking.net/media/global/howto/metafields-insert_dynamic_source.png "Dynamic source")

---

#### Display not supported metafields

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