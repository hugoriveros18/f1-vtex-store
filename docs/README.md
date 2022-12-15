# VTEX F1 Store Theme

This project was developed with the
minimum Boilerplate Theme that is a basic store front model based on the VTEX IO Store Framework. Likewise, the official [Formula One](https://f1store4.formula1.com/es/) page was selected as a reference page, where it sought to replicate its functionality and styles in a responsive manner.

## Configuration

### Step 1 -  Basic setup

Access the VTEX IO [basic setup guide](https://vtex.io/docs/getting-started/build-stores-with-store-framework/1) and follow all the given steps. 

By the end of the setup, you should have the VTEX command line interface (Toolbelt) installed along with a developer workspace you can work in.

### Step 2 - Cloning the VTEX F1 Store Theme repository

[Clone](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository) this repository to your local files to be able to effectively start working on it.

Then, access the repository's directory using your terminal. 

### Step 3 - Editing the `Manifest.json`

Once in the repository directory, it is time to edit the  VTEX F1 Store Theme `manifest.json` file. 

Once you are in the file, you must replace the `vendor` and `account` values. `vendor` is the account name you are working on and `account` is anything you want to name your theme. For example:

```json
{
  "vendor": "itgloberspartnercl",
  "name": "store-theme",
}
```

### Step 4 -  Installing required apps

In order to use Store Framework and work on your store theme, it is needed to have both `vtex.store-sitemap` and `vtex.store` installed.

Run  `vtex list`  and check whether those apps are already installed. 

If they aren't, run the following command to install them: `vtex install vtex.store-sitemap vtex.store -f`

### Step 5 -  Uninstalling any existing theme

By running `vtex list`,  you can verify if any theme is installed.

It is common to already have a `vtex.store-theme`  installed when you start the store's front development process. 

Therefore, if you find it in the app's list, copy its name and use it together with the command `vtex uninstall`. For example:

```json
vtex uninstall vtex.store-theme
```

### Step 6- Review the necessary dependencies and builders

For the correct functioning of the project it is important to make sure that the following builders, dependencies, peer dependencies and custom apps are declared in the manifest.json
### Builders

```json
{
  "styles": "2.x",
  "store": "0.x",
  "sitemap": "0.x",
  "docs": "0.x",
  "assets": "0.x"
}
```
### Dependencies
```json
{
  "vtex.store": "2.x",
    "vtex.store-header": "2.x",
    "vtex.product-summary": "2.x",
    "vtex.store-footer": "2.x",
    "vtex.store-components": "3.x",
    "vtex.styleguide": "9.x",
    "vtex.slider": "0.x",
    "vtex.carousel": "2.x",
    "vtex.shelf": "1.x",
    "vtex.menu": "2.x",
    "vtex.minicart": "2.x",
    "vtex.product-details": "1.x",
    "vtex.product-kit": "1.x",
    "vtex.search-result": "3.x",
    "vtex.login": "2.x",
    "vtex.my-account": "1.x",
    "vtex.flex-layout": "0.x",
    "vtex.rich-text": "0.x",
    "vtex.store-drawer": "0.x",
    "vtex.locale-switcher": "0.x",
    "vtex.product-quantity": "1.x",
    "vtex.product-identifier": "0.x",
    "vtex.product-specification-badges": "0.x",
    "vtex.product-review-interfaces": "1.x",
    "vtex.telemarketing": "2.x",
    "vtex.order-placed": "2.x",
    "vtex.stack-layout": "0.x",
    "vtex.tab-layout": "0.x",
    "vtex.responsive-layout": "0.x",
    "vtex.slider-layout": "0.x",
    "vtex.iframe": "0.x",
    "vtex.breadcrumb": "1.x",
    "vtex.sticky-layout": "0.x",
    "vtex.add-to-cart-button": "0.x",
    "vtex.modal-layout": "0.x",
    "vtex.store-link": "0.x",
    "vtex.search": "2.x",
    "vtex.store-icons": "0.x",
    "vtex.checkout-summary": "0.x",
    "vtex.disclosure-layout": "1.x",
    "vtex.product-list": "0.x",
    "vtex.product-price": "1.x",
    "vtex.product-specifications": "1.x",
    "vtex.list-context": "0.x",
    "vtex.store-newsletter": "1.x",
    "vtex.store-form": "0.x",
}
```
### PeerDependencies

```json
{
  "vtex.mega-menu": "2.x"
}
```

### Custom Apps

For custom apps to work correctly you must clone them from their respective repositories and link them to the store theme. Below you can find the repository of each one with their documentation.

[Whatsapp Button](https://github.com/hugoriveros18/vtex-whatsapp-button)

[Quick Order](https://github.com/hugoriveros18/vtex-quick-order)

[Add To Cart Information](https://github.com/hugoriveros18/vtex-add-to-cart-info)

[Countdown](https://github.com/hugoriveros18/vtex-custom-countdown)


```json
{
  "itgloberspartnercl.whatsapp-button": "0.x",
  "itgloberspartnercl.add-to-cart-info": "0.x",
  "itgloberspartnercl.quick-order": "0.x",
  "itgloberspartnercl.custom-countdown": "0.x",
}
```

### Step 7- Run and preview your store

Then time has come to upload all the changes you made in your local files to the platform. For that, use the `vtex link` command. 

If the process runs without any errors, the following message will be displayed: `App linked successfully`. Then, run the `vtex browse` command to open a browser window having your linked store in it.

This will enable you to see the applied changes in real time, through the account and workspace in which you are working. You should be able to see the following e-commerce website after the steps mention before:

### DESKTOP
### Home Page
<img src="https://user-images.githubusercontent.com/97485652/207725567-dc872448-8aca-4a0b-acb2-a98974919a7e.png" width="auto" style="border: solid 0.5px"/> 

### Search Result Page
<img src="https://user-images.githubusercontent.com/97485652/207725219-6b07f111-2cd8-4188-9550-18e2bb9ccc91.png" width="auto" style="border: solid 0.5px"/>

### Product Detail Page
<img src="https://user-images.githubusercontent.com/97485652/207725217-ff433253-ecd9-42e7-8326-8a110b000cbf.png" width="auto" style="border: solid 0.5px"/> 

### Minicart
<img src="https://user-images.githubusercontent.com/97485652/207725213-b1c97d34-f3b8-4be4-b8fa-d1aa4952ccec.png" width="auto" style="border: solid 0.5px"/>

### Login
<img src="https://user-images.githubusercontent.com/97485652/207725226-dd250553-dd04-4eb2-b46f-a873c5a8f853.png" width="auto" style="border: solid 0.5px"/> 

### Clients Subscription Form
<img src="https://user-images.githubusercontent.com/97485652/207725221-e1c93389-be3a-486f-aac1-a8eb94059f84.png" width="auto" style="border: solid 0.5px"/> 

### Help Custom Page
<img src="https://user-images.githubusercontent.com/97485652/207725223-b790981c-fe53-4f04-b015-4dd9c08d2aca.png" width="auto" style="border: solid 0.5px"/> 

---

### TABLET
### Home Page
<img src="https://user-images.githubusercontent.com/97485652/207726014-2a2ed6ae-8902-4572-9321-757cab4159c0.png" width="auto" style="border: solid 0.5px"/> 

### Search Result Page
<img src="https://user-images.githubusercontent.com/97485652/207726012-05562d6d-5bcd-49f9-a1c3-b4306f2a2e78.png" width="auto" style="border: solid 0.5px"/>

### Product Detail Page
<img src="https://user-images.githubusercontent.com/97485652/207726026-875b2921-934d-46dc-bab2-f614d00aa71a.png" width="auto" style="border: solid 0.5px"/> 

### Minicart
<img src="https://user-images.githubusercontent.com/97485652/207726024-96672c87-ef4d-418c-a950-750b60d7987d.png" width="auto" style="border: solid 0.5px"/>

### Login
<img src="https://user-images.githubusercontent.com/97485652/207726022-29f23726-fca0-4799-a33d-be6745149090.png" width="auto" style="border: solid 0.5px"/> 

### Clients Subscription Form
<img src="https://user-images.githubusercontent.com/97485652/207726017-583d53ce-e49a-4e5c-b06c-0f8a62728adb.png" width="auto" style="border: solid 0.5px"/> 

### Help Custom Page
<img src="https://user-images.githubusercontent.com/97485652/207726021-0e2ff303-8598-47a3-bcf7-f6530a282ef6.png" width="auto" style="border: solid 0.5px"/> 

---

### PHONE
### Home Page
<img src="https://user-images.githubusercontent.com/97485652/207726509-512513d3-eebf-4ffc-92c9-8e6eedf41543.png" width="auto" style="border: solid 0.5px"/> 

### Search Result Page
<img src="https://user-images.githubusercontent.com/97485652/207726529-6e4cfa75-ee57-4a86-91ff-2a46917e118d.png" width="auto" style="border: solid 0.5px"/>

### Product Detail Page
<img src="https://user-images.githubusercontent.com/97485652/207726527-e8ff0351-0979-4fb5-9ec7-cb05bbd6e24d.png" width="auto" style="border: solid 0.5px"/> 

### Minicart
<img src="https://user-images.githubusercontent.com/97485652/207726524-916441ca-ef4b-4e63-b2c5-b3620dd2dad9.png" width="auto" style="border: solid 0.5px"/>

### Login
<img src="https://user-images.githubusercontent.com/97485652/207726522-1e7880ca-ae22-4a53-9148-b8bc30f91840.png" width="auto" style="border: solid 0.5px"/> 

### Clients Subscription Form
<img src="https://user-images.githubusercontent.com/97485652/207726513-22f93ba4-9d41-4360-8230-280c3ae9ed06.png" width="auto" style="border: solid 0.5px"/> 

### Help Custom Page
<img src="https://user-images.githubusercontent.com/97485652/207726517-d3741f8e-2f86-4028-ab02-e1223e05fa77.png" width="auto" style="border: solid 0.5px"/> 

# Contributors ✨

1. Hugo Felipe Riveros Fajardo
