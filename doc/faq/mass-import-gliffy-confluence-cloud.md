---
title: Mass import Gliffy diagrams to draw.io in Confluence Cloud
layout: page
faq: true
categories: [Confluence Cloud, Gliffy, Import]
---

As an administrator, you can convert all of the Gliffy diagrams in your Confluence Cloud instance into draw.io diagrams with one click.

1. Go to the Confluence Settings in your Cloud instance.
2. Select on _draw.io Gliffy Import_ in the left menu.
3. Click on the _Start Import_ button and wait for the import to complete.

<img src="/assets/img/blog/confluence-cloud-start-gliffy-import.png" style="width=100%;max-width:400px;height:auto;" alt="Start the Gliffy mass import to draw.io diagrams in Confluence Cloud">

**Important**

* Keep your browser tab open while the import is in progress.
* The time required for conversion depends on how many Gliffy diagrams are in your Confluence Cloud instance.
* The conversion will not affect the performance of your Confluence instance. To minimise user confusion however, it's best to mass import Gliffy diagrams when as few users are active as possible.
* Previously imported diagrams will not be imported again.

## Gliffy to draw.io c​onversion log

You'll see a running log of the conversion. Copy this long once it is finished so you can check page and diagram content if errors occurred.

<img src="/assets/img/blog/confluence-cloud-gliffy-import-log.png" style="width=100%;max-width:400px;height:auto;" alt="Log of the Gliffy mass import to draw.io in Confluence Cloud">

No data is lost in this conversion process - a new page version will be created where Gliffy macros are replaces with draw.io macros containing the converted diagram. The original Gliffy diagram files are still attached to their page and unchanged.

* Do not delete these files - they are needed to maintain the page revision history in case you want to revert to an earlier version.

From the user's point of view, they will see the diagram in the page just as before, only now it is a draw.io diagram instead of a Gliffy diagram.


## Gliffy mass import FAQs

**When to perform the import**

Perform the conversion outside of your company's normal usage hours of the Confluence instance. It's best to carry out the whole operation when few changes are being made to pages containing diagrams.

We recommend that you remove the Gliffy license so that users do not start editing Gliffy diagrams while the process is running. Without a license, the Gliffy diagrams are effectively read-only. Please notify your users in advance.

**Diagram backups**

draw.io automatically creates a new page revision of every page that contains a Gliffy diagram. You can always revert pages to their previous versions as no Gliffy data is deleted.

**Uninstalling Gliffy**

Most Confluence Cloud administrators prefer to unambiguously recommend users diagram with on diagram editor and so uninstall the Gliffy app after migrating to draw.io. If Gliffy is already uninstalled, the mass Gliffy to draw.io import will still work, as the original diagram files are still attached to their pages.

It's best to uninstall Gliffy _after_ the mass import is completed and you have checked the result.

**Permissions**

Ensure the administrator who runs the mass import has full write permissions across _all_ spaces in your Confluence Cloud instance. 

If no such user exists, you will need to temporarily elevate an administrator to have those permissions for the duration of the import.

_This is the most common cause of 403 errors._

**Troubleshooting**

Make sure you always test the mass Gliffy import on a test instance with your production data first. If you encounter any issues during this mass import, please email support@draw.io and send the Gliffy Import Report text file as an attachment to your email.