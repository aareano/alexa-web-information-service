## Alexa Web Information Service Api Samples

This repo contains code samples in various languages to make signed requests
to the Alexa Web Information Service API on AWS Marketplace.

The samples are designed to demonstrate how to make a request to Alexa Web
Information Service using the API user credentials and API plan key that are
provided after subscribing to the service. You may subscribe to Alexa Web
Information Service at
https://aws.amazon.com/marketplace/seller-profile?id=4a9dbf38-88b1-4e87-a459-271154a77d2e.
(Note that you must have an AWS account with a valid credit card)

Alexa's Web Services can help you create innovative web solutions and services
based on Alexa's vast repository of information about the web. Developers,
researchers, web site owners, and merchants can incorporate information about
web sites directly into their own web sites or services. Users can access web
site traffic data, related links, and a wide variety of other functionality
and data.

#### URL Information

The URL Information action gives developers direct access to information
pertaining to web pages and sites on the web that Alexa Internet has gathered
through its extensive web crawl and web usage analysis. Examples of
information that can be accessed are site popularity and detailed
usage/traffic stats.

#### Historical Web Traffic

The Historical Traffic action gives programmatic access to web site traffic
rank, reach, and page views going back four years. Use this action to compare
a web site’s popularity over time, identify trends, or display graphs of
traffic.

#### Sites Linking In

The Sites Linking In action returns the sites linking to a specified web site.

#### Browse Category

The Browse Category and Browse Listings actions return the top sites within a
category.

## License Summary

This sample code is made available under the MIT license.

## Python

Python Sample for Alexa Web Information Service

This sample will make a request to the Alexa Web Information Service using
the API user credentials and API plan key.

Tested with Python v3.7.2 and Python v2.7.14

1. Subscribe to the Alexa Web Information Service at https://aws.amazon.com/marketplace.
   (Note that you must have an AWS account with a valid credit card)
2. Register or login to the Alexa Developer Portal and copy the API Key shown on the page.
3. Uncompress the zip file into a working directory.
4. Install requirements:

```bash
pip install -r requirements.txt
```

5. Run:

```bash
python3 awis.py -u <USER> --key=<API_KEY> --action=urlInfo --options="&ResponseGroup=Rank&Url=sfgate.com"
```

If you are getting "Not Authorized" messages, you probably have one of the
following problems:

1. Your API registration might not be complete. Return to the AWS Marketplace
   listing page and confirm you are subscribed to the product.

2. If you are getting "Request Expired" messages, please check that the date
   and time are properly set on your computer.

Copyright and License All content in this repository, unless otherwise stated,
is Copyright © 2019 Amazon.com, Inc. or its affiliates. All Rights Reserved.

Except where otherwise noted, all examples in this collection are licensed
under the MIT license. The full license text is provided in the LICENSE file
accompanying this repository.
