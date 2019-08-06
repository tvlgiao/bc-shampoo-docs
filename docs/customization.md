# Customization

This page will explain all configuration available and how to edit each section appear on theme. Let's view the first homepage.

![Homepage of Default Style](img/home1.jpg)







## Top Banner

![Top Banner](img/home1-top-banner.png)

The top banner can be showed / edited in admin page > __Marketing__ > __Banners__. When you add / edit remember to choose __Location__ is __Top of Page__.

### Colors Customization

To customize colors of this section, go to admin page > __Storefront Design__ > __My Themes__, click button __Customize__ of the current theme to open the Theme Editor. 

![Click customize theme](img/click-customize-theme.png)

Look into the options showing below:

![Theme editor top banner](img/theme-editor-top-banner.png)



## Header

### Header Styles
This theme support 3 different header styles:
- Logo at left
- Logo at right
- Logo at center

![Header Logo at left](img/home1-header-left.png)

![Header Logo at right](img/home1-header-right.png)

![Header Logo at center](img/home1-header-center.png)

To configure, open the __Theme Editor__, scroll down to section __Logo__, click to expand the logo options. Choose a certain option of __Logo position__, then click __Refresh__ button appear after.

![Change logo position](img/change-logo-position.png)

### User navigation Customization

To customize User navigation of the header section, look into the options showing below in the Theme Editor:

![User navigation Customization](img/theme-editor-header-user-navigation.png)

### Main navigation Customization

To customize Main navigation of the header section, look into the options showing below in the Theme Editor:

![Page navigation Customization](img/theme-editor-header-page-navigation.png)

## Main Slideshow / Carousel

### Edit the slideshow

Edit the slideshow in admin page > __Storefront Design__ > __Design Options__:

![Edit homepage carousel](img/edit-homepage-carousel.png)

### Change position of text content

The theme supports showing slideshow content like heading, text, button on __left__, __right__ or __center__ of the image. To configure this option, open Theme Editor, Look into section Carousel, click to expand:

![Edit position of each carousel slide](img/theme-editor-carousel-desc-position.png)

Choose position of each slide you want to change.

### Colors Customization

To customize color of the slideshow's elements, look into section __Carousel__ in the Theme Editor:

![Theme editor carousel](img/theme-editor-carousel.png)

### Hide the slideshow

To hide the slideshow on homepage, uncheck on the checkbox __Show Carousel__ in section __Carousel__ of the Theme Editor.

## Two Banner

![Products section](img/index-two-banner-section.png)
To change the image url. Edit its values as you want.
![Products section](img/index-two-banner-section-edit.png)

## Products section 
![Products section](img/index-products-section-new.png)
![Products section](img/index-products-section-furure.png)
![Products section](img/index-products-section-top.png)
To change the heading text, Columns number to show, Type, edit in The products section. Edit its values as you want.

![Products section](img/index-products-section-edit.png)


## Recent Blog Posts

![Recent blog posts](img/home1-blog.jpg)

This block show the most recent blog posts.

### Customize heading text and other text

To change the heading text, read more text and date format, edit in The Blog section. Edit its values as you want.

![Edit recent blog text in the language file](img/edit-blog.png)

## Instagram Photos

![Instagram Photos block](img/home1-instagram.jpg)

### Get your own User ID, Client ID, Access Token

In order to display your Instagram photos on your website, you will need to get the __User ID__, __Client ID__ and __Access Token__ from __Instagram Developer__ portal.

#### 1. Create your own Client ID

Open the URL <https://www.instagram.com/developer/> in your browser.

Login to your Instagram account.

Click button __Register Your Application__: 

![Instagram register your application](img/instagram-register.png)

Click button __Register a New Client__: 

![Instagram new client](img/instagram-register-new-client.png)

Enter all required info on the form. 

![Instagram registration form](img/instagram-registration-form.png)

Note that __Valid redirect URIs__ should be exactly `http://127.0.0.1` as recommended as it will be used in the next step.

After submitting the form you will get back to the previous page with a new __Client ID__ is created.

![Instagram Manage Clients](img/instagram-manage-clients.png)

Save this __Client ID__ value, it will be used to configure the Instagram Photos block.

#### 2. Retrieve your Access Token

Click button __Manage__ on your the client app created previously. Open __Security__ tab, uncheck __Disable Implicit OAuth__ checkbox:

![Manage client - security tab](img/instagram-implicit-oauth.png)

Click __Update Client__ button to complete.

Now open your web browser with the URL: 

```plain
https://api.instagram.com/oauth/authorize/?client_id=CLIENT-ID&redirect_uri=http://127.0.0.1&response_type=token
```

where `CLIENT-ID` is replaced by your __Client ID__ number created previously.

Click __Authorize__ button to grant access permission:

![Authorize client app](img/instagram-authorize.png)

Instagram will redirect you to an error page with the URL similiar: 

![URL contains access token](img/instagram-get-code.png)

The text after `access_token=` is the __Access Token__ you want to get. Save it for the next step.

#### 3. Retrieve your User ID

Open the link below on your web browser:

```plain
https://api.instagram.com/v1/users/self/?access_token=ACCESS-TOKEN
```
Where `ACCESS-TOKEN` is replaced by your real __Access Token__ just received previously.

![User ID code](img/instagram-get-userid.png)

The number in `"id": "..."` is your __User ID__.

### Display your Instagram photos

To display our own Instagram photos, in the Instagram section. input your real code:

- `access_token`: is your Instagram __Access Token__.

![Edit instagram in the language file](img/edit-instagram.png)

## Footer - Newsletter

![Newsletter](img/home1-newsletter.png)

### Change text

To change text appear on this section you can edit the language file as instruction below:

From admin page > __Storefront Design__ > __My Themes__, click button __Advanced__ > __Edit Theme Files__ of the current theme:

![Edit theme files](img/edit-theme-files.png)

From the left navigation, click to edit the language file (e.i `en.json`):

![Edit language file](img/edit-language-file.png)

See the section `Newsletter` you can edit as you want:

![Edit language newsletter](img/edit-language-newsletter.png)


## Social Media Icons
![Theme editor payment icons](img/theme-editor-social-icons.png)

You will need to configure which icons to appear in admin panel > __Storefront Design__ > __Design Options__, input your social links in __Social Media__ section.




## Payment Icons

![Theme editor payment icons](img/theme-editor-payment-icons-edit.png)

![Theme editor payment icons](img/theme-editor-payment-icons.png)

To show/hide payment icons, go to Theme __Editor__ > __Payment Icons__ secitons, check or uncheck any icons you want to show or hide.

## Credit Links

![Theme editor credit links](img/theme-editor-credits.png)

To show/hide the credit links, go to Theme Editor > __Footer__ section, tick or untick the checkboxes as showing above.


## Assign different product layout to a specific product page

Theme has 2 product layouts: __default__ and __Fullwith with Lightbox__.

Product layout fullwidth:

![Product layout fullwidth](img/product-layout-fullwidth.jpg)

To assign a product layout, edit your product in the admin panel. In tab __Order Details__, choose __Template Layout File__ with the layout out want:

![Assign product layout](img/assign-product-layout.png)

## Assign different category layout to a specific category page

Theme has 2 category layout: __default__ and __Fullwidth__.

Category layout fullwidth:

![Category layout fullwidth](img/category-layout-fullwidth.jpg)

To assign a category layout, edit your category in the admin panel. Choose __Template Layout File__ with the layout out want:

![Assign category layout](img/assign-category-layout.png)


## Show custom product labels

![Product labels](img/product-labels.jpg)

Turn on displaying product labels in the __Theme Editor__ > __Products section__, tick on the checkbox __Show custom label using custom field 'card_label'__ and __choose Display Product Sale Badges__ as __Top Left__.

![Theme editor products options](img/theme-editor-products-show-options.png)

![Theme editor product sale badges](img/theme-editor-product-sale-badges.png)

Edit your product in the admin panel to add custom label:

![Edit product custom fields](img/edit-product-custom-fields.png)

Add a custom label named `card_label` and enter label text in the value input box.

## Show color swatches on product card:

![Color swatches on product card](img/product-card-color-swatches.png)

To display color watches on product card, open __Theme Editor__ > __Products section__, tick on the checkbox __Show color swatches using custom field 'card_color'__.

![Theme editor products options](img/theme-editor-products-show-options.png)

Edit your product in the admin panel to add custom label:

![Edit product custom fields](img/edit-product-custom-fields.png)

Add a custom label named `card_color` and enter color hex code in the value input box seperator by commas.

## Add our own CSS (Sass) code

To add your own custom CSS code you can edit the file `assets/scss/_theme-custom.scss_` in __Edit Theme Files__ editor:

![Edit file _theme-custom.scss](img/edit-file-theme-custom-css.png)

__Note: __

- Copy / backup this file for future theme upgrade.
- Add custom CSS code required CSS (or Sass) programming skill. It's not recommended for new users.
