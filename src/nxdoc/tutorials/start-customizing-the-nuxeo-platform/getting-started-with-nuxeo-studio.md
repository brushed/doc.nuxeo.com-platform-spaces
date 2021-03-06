---
title: Getting Started with Nuxeo Studio
review:
    comment: ''
    date: '2015-12-01'
    status: ok
details:
    howto:
        excerpt: Learn how to start working with Nuxeo Studio.
        level: Beginner
        tool: Nuxeo Studio
        topics: 'Document type, Style'
labels:
    - howto
    - studio
toc: true
confluence:
    ajs-parent-page-id: '14256538'
    ajs-parent-page-title: Start Customizing the Nuxeo Platform
    ajs-space-key: NXDOC
    ajs-space-name: Nuxeo Platform Developer Documentation
    canonical: Getting+Started+with+Nuxeo+Studio
    canonical_source: 'https://doc.nuxeo.com/display/NXDOC/Getting+Started+with+Nuxeo+Studio'
    page_id: '20518152'
    shortlink: CBU5AQ
    shortlink_source: 'https://doc.nuxeo.com/x/CBU5AQ'
    source_link: /display/NXDOC/Getting+Started+with+Nuxeo+Studio
tree_item_index: 100
history:
    -
        author: Solen Guitter
        date: '2016-09-07 09:23'
        message: ''
        version: '26'
    -
        author: Solen Guitter
        date: '2016-09-07 09:12'
        message: 'NXDOC-857: remove nuxeo.io'
        version: '25'
    -
        author: Manon Lumeau
        date: '2016-05-06 13:02'
        message: ''
        version: '24'
    -
        author: Manon Lumeau
        date: '2016-05-06 12:53'
        message: ''
        version: '23'
    -
        author: Solen Guitter
        date: '2016-04-14 12:39'
        message: Update Studio menu labels
        version: '22'
    -
        author: Solen Guitter
        date: '2016-03-31 15:41'
        message: Fix links
        version: '21'
    -
        author: Manon Lumeau
        date: '2016-03-31 09:26'
        message: Fix links
        version: '20'
    -
        author: Julie Allouch
        date: '2016-03-29 19:51'
        message: ''
        version: '19'
    -
        author: Solen Guitter
        date: '2016-03-02 09:32'
        message: ''
        version: '18'
    -
        author: Solen Guitter
        date: '2016-03-02 09:31'
        message: ''
        version: '17'
    -
        author: Bertrand Chauvin
        date: '2016-01-07 11:00'
        message: Update titles to fix anchor links
        version: '16'
    -
        author: Manon Lumeau
        date: '2015-10-01 15:51'
        message: ''
        version: '15'
    -
        author: Manon Lumeau
        date: '2015-10-01 15:51'
        message: ''
        version: '14'
    -
        author: Solen Guitter
        date: '2015-08-03 07:39'
        message: ''
        version: '13'
    -
        author: Manon Lumeau
        date: '2015-07-31 13:50'
        message: ''
        version: '12'
    -
        author: Manon Lumeau
        date: '2015-07-31 13:20'
        message: ''
        version: '11'
    -
        author: Manon Lumeau
        date: '2014-12-29 16:26'
        message: ''
        version: '10'
    -
        author: Manon Lumeau
        date: '2014-11-07 10:48'
        message: ''
        version: '9'
    -
        author: Manon Lumeau
        date: '2014-11-07 10:48'
        message: ''
        version: '8'
    -
        author: Manon Lumeau
        date: '2014-11-07 10:47'
        message: ''
        version: '7'
    -
        author: Manon Lumeau
        date: '2014-11-07 10:44'
        message: ''
        version: '6'
    -
        author: Manon Lumeau
        date: '2014-11-07 10:44'
        message: ''
        version: '5'
    -
        author: Manon Lumeau
        date: '2014-11-07 10:39'
        message: ''
        version: '4'
    -
        author: Manon Lumeau
        date: '2014-11-07 10:35'
        message: ''
        version: '3'
    -
        author: Manon Lumeau
        date: '2014-11-06 12:23'
        message: ''
        version: '2'
    -
        author: Manon Lumeau
        date: '2014-11-06 12:21'
        message: ''
        version: '1'

---
This page explains how to start customizing the Nuxeo Platform using Nuxeo Studio. It will guide you through the steps to:

*   Get a Nuxeo Studio project using Nuxeo Online Services
*   Get a running Nuxeo Platform instance
*   Change the logo of your Nuxeo Platform instance
*   Create a new Contract document type in Studio

Nuxeo Studio is a Nuxeo tool provided as part of the Nuxeo Online Services subscription offer. If you are a Nuxeo customer, you should already have a username/password to connect and access to your Studio project. Otherwise, we provide a 30-day trial offer so you can discover Nuxeo Studio and its configuration capabilities.

## Step 1 - Get a Nuxeo Platform Instance

The Nuxeo Platform is available in different packages. Here let's use the ZIP archive.

Installing the Nuxeo Platform using the&nbsp;[.zip package](http://www.nuxeo.com/downloads/)&nbsp;installs the Nuxeo Platform only. External dependencies must be&nbsp;[installed separately]({{page page='installing-and-setting-up-related-software'}}).

**To install and start the Nuxeo Platform ZIP archive:**

1.  Unzip the .zip archive using your favorite tool.
2.  Click on the Start Nuxeo.command to start the server.
3.  In a browser, go to [http://localhost:8080/nuxeo](http://localhost:8080/nuxeo).
4.  Fill in the information in the configuration wizard steps.
5.  At the Nuxeo Online Services step, provide your Nuxeo Online Services credentials if you already have a Nuxeo Online Services account or register to the 30-day trial offer.

    1.  Provide a valid email address or else registration will not be completed.
    2.  Confirm registration by clicking on the link sent to the email address you provided.
        Your Online Trial account is created.
        You can now access Nuxeo Studio by clicking on the&nbsp;link&nbsp;provided in the last email received.
6.  Click on&nbsp;**Start**&nbsp;at the final step.&nbsp;
    Your application is ready to use.&nbsp;
    You now need to activate development mode so as to enjoy the hot reload of your Nuxeo Studio configuration.

**To activate development mode:**

1.  When the application is started, log in with the Administrator / Administrator credentials.
2.  Click on&nbsp;**Admin Center**&nbsp;>&nbsp;**Update Center**.
    The Nuxeo Studio tab is displayed.
3.  Click on the&nbsp;**Enable**&nbsp;button to activate development mode.
4.  Click on the&nbsp;**Restart Server**&nbsp;button displayed on top of the Admin Center.
    The Nuxeo Platform instance restarts. You can then enjoy your Nuxeo Studio configuration without restarting your server.

Once your project registered on Online Services, you can start customizing your Nuxeo Application. The first&nbsp;customizations&nbsp;occur in Nuxeo Studio, where you can easily create new&nbsp;[document types]({{page space='studio' page='documents'}}),&nbsp;[content views]({{page space='studio' page='content-views'}})&nbsp;, etc. Here, we will change the logo and then create a document type "Contract".

You can now access Nuxeo Studio from Online Services by clicking on this&nbsp;link: [connect.nuxeo.com/nuxeo/](http://connect.nuxeo.com/nuxeo/).

## Step 2 - Edit the Logo

Goal is to change the logo displayed in the banner of the Nuxeo Platform application. You must preliminary have a logo in PNG or JPG.

### Studio Customization

**Change the logo:**

1.  In Studio's left menu, click on the&nbsp;**Branding**&nbsp;section.
2.  Click on the&nbsp;**New**&nbsp;button.
3.  In Feature ID field, type "MyBranding" and click on the&nbsp;**Next**&nbsp;button.
4.  In **Main Pages** tab:

    1.  Check-box "Set as default branding" must be checked.
    2.  Click on the&nbsp;**Select Resource**&nbsp;button of the "Logo image" field.
        A "Select Resource" window pops up. It shows a list of images imported with the DM template.
    3.  Click on&nbsp;**Choose File**&nbsp;and select an image from your desktop.
    4.  Click on the&nbsp;**Upload&nbsp;**button.
        The selected image is uploaded to Studio, added to the list of available images and selected.
    5.  Click on the&nbsp;**Ok**&nbsp;button at the bottom of the popup window.
        The path to the uploaded image is displayed next to the&nbsp;**Select resource**&nbsp;button.

### Deploying Changes on Your Nuxeo Platform Instance

1.  Go to your Nuxeo Platform instance, typically available&nbsp;at <span class="s2">[http://localhost:8080/nuxeo](http://localhost:8080/nuxeo).
    </span>
2.  Connect as Administrator with Administrator password.
3.  Click on **Admin Center** > **Update Center** > **Nuxeo Studio**.
4.  Click on the **Update** button.
    Your logo is updated.

## {{> anchor 'contract-doc-type'}}Step 3 - Create a Contract Document Type&nbsp;

Here we want to create a document type "Contract" that will hold specific metadata related to the notion of contract: contract owner, starting date, policy.

### Studio Customization

1.  Unfold the&nbsp;**Content Model**&nbsp;item of the Studio tree, click on&nbsp;**Document Types** and click the&nbsp;**New**&nbsp;button.
2.  Fill in the creation form and click on&nbsp;**Next**:
    *   ID: Contract
    *   Extends: File
    *   Label: Contract
    *   Description: Contract document type for internal use.Your document type is created.
3.  Fill in the&nbsp;[ **Definition**&nbsp;tab]({{page space='studio' page='documents'}}):
    ![]({{file name='definition_contract.png'}} ?w=600,h=365,border=true)
4.  Fill in the&nbsp;[&nbsp;**Schema**&nbsp;tab]({{page space='studio' page='schemas'}})&nbsp;with the following metadata:&nbsp;
    ![]({{file name='schema_contract.png'}} ?w=600,border=true)

5.  Specify the&nbsp;[form that will be used to create the document (aka creation layout)]({{page space='studio' page='form-layouts'}}):&nbsp;
    1.  Click on the&nbsp; icon&nbsp;![]({{file name='delete.gif' space='studio' page='studio-icons-index'}})&nbsp;to remove the WARNING and Description widgets.
    2.  Drag and drop the fields "Owner", "Start" and "Policy" from the schema Contract to the grid.
    3.  Click on&nbsp;_&nbsp;![]({{file name='editor_area.gif' space='studio' page='studio-icons-index'}})_ &nbsp;if you want to edit their label and click on the popup&nbsp;**Save**&nbsp;button.&nbsp;
        ![]({{file name='creation_layout_contract.png'}} ?w=580,border=true)
6.  On the Edit layout (the form used to update the metadata of the document):
    1.  Click on the&nbsp;button&nbsp;**Import Layout**&nbsp;and select&nbsp;**Import 'create' layout**.
    2.  Click on the button&nbsp;**Add Row**.&nbsp;
    3.  Drag and drop the field Reminder from the schema Contract to the grid.
    4.  Click on&nbsp;_&nbsp;![]({{file name='editor_area.gif' space='studio' page='studio-icons-index'}})_ &nbsp;if you want to edit the widget label and click on the popup&nbsp;**Save**&nbsp;button.&nbsp;
        ![]({{file name='edit_layout_contract.png'}} ?w=600,border=true)
7.  Repeat the Edit layout steps on the View Layout.
8.  Click on&nbsp;**Save.**

### Deploying Changes on Your Nuxeo Platform Instance

1.  Go to your Nuxeo Platform instance, typically available&nbsp;at&nbsp;<span class="s2">[http://localhost:8080/nuxeo](http://localhost:8080/nuxeo).
    </span>
2.  Connect as Administrator with Administrator password.
3.  Click on&nbsp;**Admin Center**&nbsp;>&nbsp;**Update Center**&nbsp;>&nbsp;**Nuxeo Studio**.
4.  Click on the&nbsp;**Update**&nbsp;button.
5.  Go in a workspace and create a new Contract.
    ![]({{file name='create_contract.png'}} ?w=350,h=271,border=true)

&nbsp;

{{#> callout type='info' }}

You are now ready to use Nuxeo Studio!&nbsp;You can:

*   Go deeper with learning more of Nuxeo Studio and Nuxeo Platform, by following a&nbsp;[complete tutorial]({{page page='first-steps-with-studio-technical-documentation-tutorial'}}).
*   Go to the next step of this quick start, so as to discover how you can contribute new Java development to the server.

{{/callout}}
