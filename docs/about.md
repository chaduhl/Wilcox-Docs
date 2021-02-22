# About

## How the Site is Set Up

The Wilcox site runs on an independent CPanel server at the University of Kansas and employs Omeka S as a content management system. The following documentation is intended as a guide for students and faculty of the Department of Classics with information about uploading, updating, and managing items within the collection as well as individual static pages. This documentation aims to extend the more general [Omeka S documentation](https://omeka.org/s/docs/user-manual/). 

The administrator of the site has two primary ways of accessing and editing the site:

- the server-side backend (CPanel), which is used primarily for accessing the server’s file system and uploading batch files. and the Omeka S backend. Accessible at [http://wilcox.ku.edu/cpanel](http://wilcox.ku.edu/cpanel).
- The Omeka S backend, which is used for managing items in the collection and static site pages. Accessible at [http://wilcox.ku.edu/admin](http://wilcox.ku.edu/admin).

## Intro to CPanel

CPanel is the interface for working with the server at KU which hosts the Wilcox site. It allows one to view and configure the settings of the server via a graphical interface. Most of the features of CPanel will not be relevant for you since they are largely managed by KU IT.

The most important feature, however, is the file explorer. This is where one can explore and edit the files that make the site work. For the average person working with the collection, the CPanel file explorer will be most relevant in its capacity for batch uploading images. 

## Intro to Omeka S

The Wilcox Collection is organized by **Item Sets**, so that you may browse items that are similar to each other, but you may also view all the items together. You can access these from the **Admin Dashboard**, by clicking either **Items** or **Item Sets**.
Here is a list of the **Item Sets**:

- **Artifact Collection**
- **Numismatic Collection**
- **Plaster Cast Collection**
- **Inscriptions**

> **Note:**
> The 3D models page is just a static page that has embedded code to display the models which are hosted on Sketchfab. 

Additionally, there are hidden **Item Sets** which facilitate how the site organizes metadata. For example, one hidden **Item Set** is **Material**, which contains item entries for all the types of material that coins can be made from. Having these item entries allow us to link together coins that are made from the same material and thus allows public users to sort items by their material. Public users of the site do not need to see these items, and so they are hidden from view.

## After Updating the Server Password

It is very important to keep track of the passwords for the site since there are quite a few and all with different permissions. 

After updating the password for the server, the `database.ini` file in Omeka S must be edited to reflect the change. The file can be found here:

    public_html/
        config/
            database.ini

## Introduction to Metadata

Omeka S was chosen for its robust content management system and its foundations in linked-open data. The site uses a custom XML ontology, named **Wilcox Collection Ontology**, to organize and maintain the metadata (e.g. an item’s physical dimensions, conservation state, description, etc.) for all objects within the collection. This method for organizing the data allows for future flexibility and sharing of the collection with other scholarly projects. 

Every information field that should be used for items is part of this ontology. Full documentation of the ontology can be found under [**Wilcox Collection Ontology**](wcx_ontology.md).

