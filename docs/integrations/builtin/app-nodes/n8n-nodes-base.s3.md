---
title: S3
description: Documentation for the S3 node in n8n, a workflow automation platform. Includes details of operations and configuration, and links to examples and credentials information.
contentType: integration
---

# S3

Use the S3 node to automate work in non-AWS S3 storage and integrate S3 with other applications. n8n has built-in support for a wide range of S3 features, including creating, deleting, and getting buckets, files, and folders. For AWS S3, use [AWS S3](/integrations/builtin/app-nodes/n8n-nodes-base.awss3/).

Use the S3 node for non-AWS S3 solutions like:

* [MinIO](https://min.io/){:target="_blank" .external-link}
* [Wasabi](https://wasabi.com/){:target="_blank" .external-link}
* [Digital Ocean spaces](https://www.digitalocean.com/products/spaces){:target="_blank" .external-link}

On this page, you'll find a list of operations the S3 node supports and links to more resources.

/// note | Credentials
Refer to [S3 credentials](/integrations/builtin/credentials/s3/) for guidance on setting up authentication. 
///
/// note | Examples and templates
For usage examples and templates to help you get started, take a look at n8n's [S3 integrations](https://n8n.io/integrations/s3/){:target="_blank" .external-link} list.
///

## Operations

* Bucket
    * Create a bucket
    * Delete a bucket
    * Get all buckets
    * Search within a bucket
* File
    * Copy a file
    * Delete a file
    * Download a file
    * Get all files
    * Upload a file
    
    /// note | Attach file for upload
    To attach a file for upload, use another node to pass the file as a data property. Nodes like the [Read/Write Files from Disk](/integrations/builtin/core-nodes/n8n-nodes-base.filesreadwrite/) node or the [HTTP Request](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/) work well.
    ///

* Folder
    * Create a folder
    * Delete a folder
    * Get all folders

## Node reference

### Setting file permissions in Wasabi

When uploading files to [Wasabi](https://wasabi.com/){:target="_blank" .external-link}, you must set permissions for the files using the **ACL** dropdown and not the toggles.

![File permissions when using the S3 node with Wasabi](/_images/integrations/builtin/app-nodes/s3/acl_dropdown.png)

