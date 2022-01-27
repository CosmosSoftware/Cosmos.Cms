# Cosmos CMS (Editor and Publisher)

Note: This is the full repository for Cosmos Editor and Publisher.  Please see also our [stand-alone Publisher repository](https://github.com/CosmosSoftware/CDT.Cosmos.Cms.Website).  Most users will want to extend that project.

[![ubunto build](https://github.com/CosmosSoftware/Cosmos.Cms/actions/workflows/dotnet.yml/badge.svg)](https://github.com/CosmosSoftware/Cosmos.Cms/actions/workflows/dotnet.yml) [![CodeQL](https://github.com/CosmosSoftware/Cosmos.Cms/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/CosmosSoftware/Cosmos.Cms/actions/workflows/codeql-analysis.yml) 
[![NuGet Badge](https://buildstats.info/nuget/CDT.Cosmos.Cms.Common)](https://www.nuget.org/packages/CDT.Cosmos.Cms.Common/)

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://cosmos.moonrise.net/get_started/install)

# What Makes Cosmos Different?

Plenty of content management systems (CMS) already exist that are easy to use as they allow for web pages to be dynamically generated and served to the public.  They are are very convenient.

Not infrequently, CMS' can have performance problems. Reason is they are generating content dynamically--which can be problematic as the number of concurrent users increases.

CMS' can be modified to handle the traffic. One common way is to install “plugins,” “modules,” “components” or “proxies” that capture dynamically generated webpages and save them as “static” files.

Now the CMS is performing much better because it is behaving more like a static website rather than a dynamic one.

Cosmos takes a different approach.  It doesn't need plugins or other add-ons to improve performance.  The reason is that at it's core is a static website where most content is stored and served from. It is then augmented with a highly efficient dynamic website to handle what needs to be generated on the fly.

The result is a CMS that performans as well as a static website without modification.

[Take 10 minutes to try out Cosmos yourself](https://cosmos.moonrise.net/get_started/install)!

# Hybrid Design

Cosmos is a high performance [web content management system](https://en.wikipedia.org/wiki/Web_content_management_system) with a hybrid design that combines a [static](https://en.wikipedia.org/wiki/Static_web_page) with a [dynamic](https://en.wikipedia.org/wiki/Dynamic_web_page) website.  The result is a _dynamic_ content management system that performes as well as a static website.

Content is managed by a third website called the "Editor."  It maintains files on the static website and makes edits to web pages on the dynamic website.  It also schedules when new content can appear and optionally manages integration with CDNs.  Additionally it can synchronize content between Cosmos instances in real time.

Performance-wise Cosmos CMS can match or slightly exceed that of a static website backed with either Amazon S3 or Azure Storage accounts.
 
Other Key features:

* Can host a single website simultaneously in AWS and Azure clouds with realtime-synchronization.
* Code editor for web developers and a WSYWIG editor for the non-technical.
* Cost effective to run.
* Optionally integrates with Akamai, Microsoft, and Verizon CDNs.

Two repositories are associated with this procject:

* The [Cosmos](https://github.com/CosmosSoftware/Cosmos.Cms) repository contains the "Editor" and the "Publisher" and all the frameworks common to each.
* The "[Cosmos Publisher](https://github.com/CosmosSoftware/Cosmos.Cms.Publisher)" repository contains a stand alone "Publisher" website.

The publisher repository is a "stock" out of the box Visual Studio application. It is turned into a "Publisher" by adding and configuring the [Cosmos Common](https://www.nuget.org/packages/CDT.Cosmos.Cms.Common/) NuGet package.

## Origin

If you would like to know the the Cosmos CMS architecture came about, please read [the origin story](https://github.com/CosmosSoftware/Cosmos.Cms/blob/main/Documentation/Origin.md).

## Developing with Cosmos

If you would like to download and work with the code in this repository, [please see our documentation on how to get started](https://github.com/CosmosSoftware/Cosmos.Cms/blob/main/Documentation/DevelopingWithCosmos.md).

## Getting Started

You can deploy Cosmos to Azure by clicking the following button (recommended) or manually install by following the directions below.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](/Documentation/Installation/AzureClickInstall.md)

This documentation is still under development, so check back for more topics as they become available.

* Setup Help
  * [Manual installation instructions](https://github.com/CosmosSoftware/Cosmos.Cms/blob/main/Documentation/Installation/Index.md)
  * Links to Docker containers containers: [Editor](https://hub.docker.com/repository/docker/toiyabe/cosmoseditor) | [Publisher](https://hub.docker.com/repository/docker/toiyabe/cosmospublisher)
* [Developing with Cosmos](/Documentation/DevelopingWithCosmos.md)

