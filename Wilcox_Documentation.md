# Wilcox Documentation

# Introduction

The Wilcox site runs on an independent CPanel server at the University of Kansas and employs Omeka S as a content management system. The following documentation is intended as a guide for students and faculty of the Department of Classics with information about uploading, updating, and managing items within the collection as well as individual static pages. This documentation aims to extend the more general [Omeka S documentation](https://omeka.org/s/docs/user-manual/). 

The administrator of the site has two primary ways of accessing and editing the site:

- the server-side backend (CPanel), which is used primarily for accessing the server’s file system and uploading batch files. and the Omeka S backend. Accessible at [http://wilcox.ku.edu/cpanel](http://wilcox.ku.edu/cpanel).
- The Omeka S backend, which is used for managing items in the collection and static site pages. Accessible at [http://wilcox.ku.edu/admin](http://wilcox.ku.edu/admin).

The Wilcox Collection is organized by **Item Sets**, so that you may browse items that are similar to each other, but you may also view all the items together. You can access these from the **Admin Dashboard**, by clicking either **Items** or **Item Sets**.
Here is a list of the **Item Sets**:

- **Artifact Collection**
- **Numismatic Collection**
- **Plaster Cast Collection**
- **Inscriptions**

Additionally, there are hidden **Item Sets** which facilitate how the site organizes metadata. For example, one hidden **Item Set** is **Material**, which contains item entries for all the types of material that coins can be made from. Having these item entries allow us to link together coins that are made from the same material and thus allows public users to sort items by their material. Public users of the site do not need to see these items, and so they are hidden from view.

# Introduction to Metadata

Omeka S was chosen for its robust content management system and its foundations in linked-open data. The site uses a custom XML ontology, named **Wilcox Collection Ontology**, to organize and maintain the metadata (e.g. an item’s physical dimensions, conservation state, description, etc.) for all objects within the collection. This method for organizing the data allows for future flexibility and sharing of the collection with other scholarly projects. 

Every information field that should be used for items is part of this ontology. Full documentation of the ontology can be found under **Wilcox Collection Ontology**.

# Create a New User

Any user designated as an admin on the site can create a new user. To do so, simply access the **Admin Dashboard** by logging in at [wilcox.ku.edu/admin](http://wilcox.ku.edu/admin). You should see the screen below:


![](https://lh3.googleusercontent.com/k_h7rVYYkX57-h6S4Upikil6VGHPfubs5OmDOmAlY56v_6H_Y7XDyCbFL4yafNZBsurPlc8tkh-uYOrsa7ED9WHSbKaxAXBa2_Gy1lmW3Xq-DSgh92_AobM9xw4qDTQvtkIBaMlC)


There will likely be a notification that there is an available update to Omeka S. Ignore this, since it is the decision of the curator and KU IT whether to install any updates.
Click on the **Users** tab under the **Admin** subheading in the menu on the left.


![](https://lh4.googleusercontent.com/o-hNX7PtYZ0f59y5WzVIlIDS23lXYQ91pl7DDQWZumG9DYXE1KY15J4Dzb3VNZSkbBiGG5HliqLEfpW4jzgNnE0S-0Av687vIlr2HcTg4hN7mi-KtG4sjL29giQHSVt9MEPPKM1Y)


Click the **Add new user** button in the top right hand corner of the screen and enter the information for the new user. You must enter an email, display name, and role for the user and check the **Is active** box.


![](https://lh6.googleusercontent.com/gGBIA4ppT3XEaQBlLf8DmLSmc8dROCSq-61OsDGA_fDY6LwFu2ISk-OQsVZzmGnx27fNFERc-UK5rr5muAahofBxVXGQ-5GtPCCV7Nj9S6QQneOuUBjP8H-opszcLFlOo_rP9TAe)


Once you click **Add** in the top right-hand corner of the screen, an email will be sent to the email address you entered asking the new user to finish creating their account by choosing a password.

# Create an Item

From the **Admin Dashboard**, navigate to Items. Click the **Add new item** button in the top right-hand corner. Select what type of item you would like to create from the **Resource Template** dropdown menu and begin filling in the fields with information about the item.

Note: Be sure to follow naming and formatting conventions as supplied by the curator.
As an example, we will create a new entry for a coin together. To begin, choose **Coin** from the **Resource Template** dropdown menu. This will automatically populate the screen with the necessary fields for entering information about a coin. 

Then, click the dropdown menu for **Class** and select **Coin**. This will be at the bottom of the dropdown menu, listed under **Wilcox Collection Ontology**.


![](https://lh3.googleusercontent.com/0GKZNXdWRTeim8VPAIrEV-8fIpsqHU3zJQ3Dwc-TK4o2LSLPdRKs4TDluilcMeBBJBgoAH_QaNqLsM3jNa_a-PdQXex4Fp3TxUleKVs9tUpweFJBkImkEP5mY-2vMcU4ZvaDgsj7)


Now that we have the information fields we need, we can begin entering information for our item. If you do not have certain information for a given field, you can delete the field by clicking the trash can icon `<i class="fas fa-trash-alt"></i>` to the right of the text box. In this case, we are creating a new item for the collection that does not have an **Old Inventory Number**, so we should delete that field.

Note: For many items, the **Old Inventory Number** field is hidden from public view and will thus have the `<i class="fas fa-eye-slash"></i>` below the trash can icon `<i class="fas fa-trash-alt"></i>`. To hide a specific field simply click the normal eye icon `<i class="fas fa-eye"></i>` to toggle that field’s visibility. 

![](https://lh5.googleusercontent.com/NKH9SG2vpIKoKf3Xc0H_4p7QnVvlaV1rFe8qy9fdLYZLxE4jHuu5FYqZBOBEAeg31xWwlda-92ZjIW4BWxk1NEYNaFuMGMxlPGGW_JWnHuFB4ypYyT9owo813EOpzCpi7fM4h5lG)


Each information field has a name, a description to explain what exactly should go into that field, and an identifier formatted as `wcx:[identifier]`. The identifier corresponds to the XML metadata schema developed for the collection. Do not worry about this, since it only pertains to the accessibility of the collection to other linked-open data projects.

Let’s assume we know the exact date for this coin to be 100 BCE. To indicate this in the data, type -100 into the date field. If the exact date is unknown, enter a date range for the object. For more information on the formatting for individual fields, see the section entitled **Wilcox Collection Ontology**.

For some information fields, you must choose another Omeka item as the field input. A good example of this is the **Material** field. To enter a coin’s material, find the **Material** information field and click the button entitled `<i class="fas fa-cubes"></i>` **Omeka resource**. 


![](https://lh5.googleusercontent.com/bHJS3vsZ6EtV54-VPvEFKCw7ax5lmyLZKlLNVIpsNQou1Ao2qMnZktzJhfMiMUHFJdisSDGczb_DrryAnJ3ilbLBuE4Md1HWoIS6xMuB5ZBr-i1R81yN-kicKOiwkKeGDE_2iG81)


Click `<i class="fas fa-cube"></i>` **Items** and select the relevant item from the menu on the right hand side:


![](https://lh5.googleusercontent.com/EJKkKa79kLIsCp3z5cBF83R2uO4TFli4qJ6l5xsqkUWD4Ggi-5TorFlvxvwycNh-UPIpbjGgiXdQt_rBHho2wgypVTKiLO9Xk6Vnm43TSyFVCf6MaDGj_gS02JXr1VC-4AQRITma)


In this case, we will filter our search to the **Material Item Set** by clicking “Filter Search” and then selecting **Material** from the “Filter by item set” dropdown menu. This will retrieve all the materials entered into the database.


![](https://lh5.googleusercontent.com/4FKvh5tjmnwEJj7oU-lhxpigzXKgXVnsYIiEkbuhpHTWR72recxecUg6KDZV0Xiy6fYfDOVXlcYuNwdRB7wa-jp_QtvxBWu8XpnSoXzPzcGAFsw0-2zn3kMx7dqFztcOYbOsqNOh)


Simply select **Silver** and then delete the blank text field from the **Material** information field. 


![](https://lh4.googleusercontent.com/ynJcJLbHlLd1p4R_IUTkt_vIHrPv9IPxDCIVU8yDCF7XIjZHRLPZiA0LPGD5OLFWsHXJPZUtnIt6FhAL6yrak6mUXIWLWiVSv5ZlBjG3FHceQOykvfzQurDHjG8FnzUgmU0rfHLc)


Finish entering the information for your item. Like **Material**, the following fields require you to choose an **Omeka resource** instead of entering a text value:

- Material
- Denomination
- Coin Wear
- Issuers

Once you have entered all the information for the new item, navigate to the Media tab at the top of the page. 


![](https://lh3.googleusercontent.com/pFkGmuHGs6puGBvL8iTdHxZjUgP_-dx4QqGlsdGk3hImvkRleSh3dRucIyAY3-wUDxfkvMq2KLMUI7G5EzDNbyrt7ZvRZPAmuB11dM6iAaSCL76LQ5MGQ3LenJdWRtLq5Yy72wET)


If images for the item have already been loaded onto the server via **Sideload**, select the **Sideload** option for as many images as there are for the new item. If you are uploading the images yourself, simply click **Upload**.

Every time you click one of the “Add Media” options on the right side of the screen, a new upload field will be added to the page. Each upload field corresponds to only one image. You may add as many upload fields as needed. It is not necessary to enter a title for the uploaded image.


![](https://lh5.googleusercontent.com/zfAHuMV3aGEWxcW_akAarVwfK-9P_0be6IUJykuCuNomj3HkMH5dAx9ufJlbqW1trh_LFuVAROishrcLNCJBZXhAen7PGDzhVjcZbqvm5xTeIDqJDnyqHe8gls8bsXVpQ0EGlK_u)


After uploading your images or choosing them via **Sideload**, navigate to the **Item Sets** tab.
Choose the relevant item set for the new item from the right hand side of the page. **Item Sets** are sorted by which user created them. For this example, we will select **Numismatic Collection**. 

Finally, all items are automatically marked as **Hidden** when first created. This indicated by the `<i class="fas fa-trash-alt"></i>` icon at the top right of the page. To mark the item as visible, simply click the icon to toggle its visibility status.


![](https://lh4.googleusercontent.com/UA_gQNtr9el5dFGF2GzzItvkvsekX7qupjdtO_l4lM2UzR61N5z4Tf8DqXtiYjKt5RwhUtw4gr1o2rfMHn6sMDa3BMe7r4e_AjI2K-wlPJJ9AutuYCW9GSnN8c27ovhMGdXI00C6)


Click the **Add** button at the top right of the page to finish creating a new item.

# Edit an Item

To edit a specific item, find the item you want to edit via the search bar, items, or item sets. If you are logged in as an admin, you can also edit the item directly from its item page on the site. Once you’ve located the item, click “Edit.”


![](https://paper-attachments.dropbox.com/s_04D4B96ED6B883620D60816BA63E30BA4100FB8A7D113F5FF9905518B80A349D_1613745415809_image.png)


This will bring you to the same type of page as when you create a new item, except most (if not all) of the information fields should be filled with information. 


![](https://paper-attachments.dropbox.com/s_04D4B96ED6B883620D60816BA63E30BA4100FB8A7D113F5FF9905518B80A349D_1613745657182_image.png)


From here, you can edit the information that needs to be amended, change the media associated with the item, change the item’s item set, etc. Be sure to click the save button in the top right after you’re finished. 

# Create a Page

From the **Admin Dashboard** click **Sites** at the top of the left-hand menu and then select “The Wilcox Classical Museum.” Omeka S is capable of hosting multiple sites on the same server, but the Wilcox Collection only requires the single “site” for its purposes. This will open up an additional set of menu options in the left-hand menu.

Click **Pages**.


![](https://paper-attachments.dropbox.com/s_04D4B96ED6B883620D60816BA63E30BA4100FB8A7D113F5FF9905518B80A349D_1613748269512_image.png)


This opens a menu of all the current pages on the site. Clicking on a page title will open that page for editing. See **Edit a Page** for more information on editing pages. 

Click **Add a New Page** at the top right of the page. Give the page a **Title**, which will be displayed as the default title when accessing the page from the public view. Then give the page a **Slug**. This is the text that will be appended to the end of the base URL for the site. Finally check **Add to Navigation**.


![](https://paper-attachments.dropbox.com/s_04D4B96ED6B883620D60816BA63E30BA4100FB8A7D113F5FF9905518B80A349D_1613748551202_image.png)


In the case of the screenshot above, the new page will be titled “Test Page” and will be accessible at http://wilcox.ku.edu/s/wilcox/page/test-page. Click **Add** in the top right corner of the page and you will be directed to the editing screen for your newly created page.


![](https://paper-attachments.dropbox.com/s_04D4B96ED6B883620D60816BA63E30BA4100FB8A7D113F5FF9905518B80A349D_1613748678406_image.png)


This is where the content for the page lives. You can see that from here you can change the previously selected **Title** and **Slug**. It is also already given a **Page Title** field.


![](https://paper-attachments.dropbox.com/s_04D4B96ED6B883620D60816BA63E30BA4100FB8A7D113F5FF9905518B80A349D_1613748775964_image.png)


Omeka S pages are set up in a block format. Instead of coding each page individually from scratch, there are specific templates that you can add to a page. The most essential of these is the **HTML** block, which is used for basic text among other things. To add an **HTML** block, simply click the **HTML** button in the **Add New Block** menu on the right-hand side of the screen. 


![](https://paper-attachments.dropbox.com/s_04D4B96ED6B883620D60816BA63E30BA4100FB8A7D113F5FF9905518B80A349D_1613748924501_image.png)


You can begin inputting your desire text. As you can see in the screenshot above, you can also style your text with the rich text formatter. Other useful blocks include:

- **Media**, used to add an image or video to a page
- **Item Showcase**, used display multiple selected objects from the collection
- **Item with metadata**, used to display a single item

Just as in all the editing screens, you can add and delete blocks at will. If you wish to delete a previously added block, click the trash can icon `<i class="fas fa-trash-alt"></i>`.

You can preview the page before making it live by clicking the **View** button in the top right of the screen. To save the page, click the **Save** button in the top right. By clicking the save button, you are publishing your edits to the live version of the site.

Once you’ve created and saved the new page. Click **Navigation** in the menu on the left-hand side of the screen. This will bring you to an overview of how the site navigation is laid out.


![](https://paper-attachments.dropbox.com/s_04D4B96ED6B883620D60816BA63E30BA4100FB8A7D113F5FF9905518B80A349D_1613749352748_image.png)


The test page we just created was added to the bottom of the navigation hierarchy. You can click and drag the page and place it wherever you desire within the hierarchy. Notice that page links can be nested inside others. For example, there are several pages nested under **About Us** which creates a dropdown menu on the public site. 

Once you’ve placed the new page in its final location, click the **Save** button.

# Edit a Page


# Batch Upload Images

Info about uploading images to server and then choosing sideload in the item edit screen.

# Wilcox Collection Ontology

A table of the custom XML ontology developed for the Wilcox Classical Museum.

