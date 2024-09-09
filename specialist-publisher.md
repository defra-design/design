
<!-- Nav
* [Interaction design and service design](/README.md)
* [What interaction designers and service designers do](/design.md)
* [Defra Design community](/community.md)
* [Tools and resources](/tools-and-resources.md)
* [Defra design standards](https://github.com/DEFRA/design-standards)
* Specialist Publisher
* [Accessibility acceptance criteria](/accessibility-acceptance-criteria.md)
* [Design crits](/design-crits.md)
* [Case studies](/case-studies.md) -->

# What is Specialist Publisher

The guide will presume you or someone in your team already have access to Whitehall Publisher or the Whitehall staging environment, Whitehall Integration.

### Overview

The publishing platform for mainstream content on GOV.UK is Whitehall Publisher. However, there are other publishing tools for types of content that cannot best be served by Whitehall Publisher. One of these is Specialist Publisher. Like Whitehall Publisher, Specialist Publisher is hosted on publishing.service.gov.uk. If you or someone in your team currently have access to either Whitehall Integration or Whitehall Publisher, you access Specialist Integration or Specialist Publisher in the same way.

Specialist Publisher allows teams to publish to GOV.UK in much the same way as in Whitehall Publisher but where content and documents are presented in a ‘finder’ functionality. This allows the published content to be filtered according to an agreed filter set including a set of specified metadata. A schema is then built for the agreed filter set. This can either be done by your team or the Specialist Publisher team at Government Digital Service (GDS) (examples of schemas). For each piece of content, metadata is presented in a blue box at the top of the content as well as in the listing in the filtered list (examples of live Specialist Finders below). The best user case for implementing a Finder is that users need to be able to find content by the way of specific meta data and filtered views.

The way that Specialist Publisher manages published content (eg research reports) is more limited than Whitehall Publisher. There is one template and when publishing content, attachments, links and images have to be added manually in the Markdown. Make sure this isn’t a problem for anyone who is going to be publishing any content in the future.
Only content published via Specialist Publisher can be displayed in the Specialist Finder. For example, if content is currently published via Whitehall Publisher, it can’t be displayed in a Specialist Finder. It would need to be republished via Specialist Publisher and then to avoid duplication the version on Whitehall Publisher would need to be deleted. The team at GDS can support with forwarding. However, any content published via Specialist Publisher does appear in GOV.UK search and can be displayed as featured content if the instance of the Specialist Finder is implemented in conjunction with a type of organisation page published via Whitehall Publisher or as linked content within a Guidance page.
The default unfiltered view of content in a Specialist Finder list is most recently published at the top of the list. In Specialist Publisher there is no functionality to select a date of publication (past or future) so if your team is planning to publish existing content as part of the set up of an instance of the Specialist Finder, you need to publish it in order of oldest first to ensure it displays in the correct order.

The implementation of a Specialist Finder requires the support of a specific team in GDS. Details below. Before talking to GDS, discuss your team’s requirements with the Head of Content in DDTS, Lucy Hartley, to establish that Specialist Publisher is the correct solution for your project.

If you have a need for volume publishing, discuss with the GDS team. They have done this before.

There is no cost to Defra to use the service.

The length of time required to deploy the service needs to be discussed with the team at GDS. Timelines can be impacted by higher priority work (eg COVID or Brexit)

### Reference

* Notes on GitHub https://github.com/alphagov/specialist-publisher
* Examples of schemas which are stored in a JSON format https://github.com/alphagov/specialist-publisher/tree/master/lib/documents/schemas
* Overview of publishing tools on GOV.UK
* Example of a prototype used on the FCERM project which could be used to get you started https://github.com/matthewsolle/FCERM-Specialist-Publisher

### Specialist Publisher team at GDS

Thomas Leese, Lead Developer thomas.leese@digital.cabinet-office.gov.uk
Jonathan Nichols, Product Manager jonathan.nichols@digital.cabinet-office.gov.uk

### Examples

https://www.gov.uk/raib-reports
https://www.gov.uk/maib-reports
https://www.gov.uk/drug-device-alerts
https://www.gov.uk/international-development-funding
https://www.gov.uk/european-structural-investment-funds
https://www.gov.uk/drug-safety-update
https://www.gov.uk/dfid-research-outputs/analysis-of-health-needs-and-health-system-response-in-the-coastal-districts-of-bangladesh
https://www.gov.uk/countryside-stewardship-grants
https://www.gov.uk/cma-cases
https://www.gov.uk/business-finance-support
https://www.gov.uk/aaib-reports

### Tips for adding content to the Markdown

#### Adding an attachment

You need to create a draft of the content you want to publish before you are able to add an attachment:

1. Add a draft of the content
2. Open it again to edit it
3. Add attachment
4. Add reference to the attachment in the Markdown at the point you want it to appear using the following code:

[InlineAttachment:file_name.filetype]
eg [InlineAttachment:A_method_for_monetising_the_mental_health_costs_of_flooding.pdf]

NB the reference needs to be the exact name of the attachment

#### Adding an image

You need to create a draft of the content you want to publish before you are able to add an image as an attachment:

1. Add a draft of the content
2. Open it again to edit it
3. Add the image you want to use as an attachemnt (it needs to be saved with the dimensions of 960x640)
4. Add reference to the attachment in the Markdown at the point you want it to appear using the following code:

![InlineAttachment:image_name.filetype]
eg ![InlineAttachment:KarinaC_StarboardWalkwayShowingStackOfHatchCoversAndGantryCrane.jpg]

NB the ! at the beginning makes it show up as an image and the reference needs to be the exact name of the attachment

#### Adding grey box

Add $CTA before and after the text you want to appear in a grey box
Example here https://www.gov.uk/maib-reports/crush-incident-on-general-cargo-vessel-karina-c-with-loss-of-1-life

### Other functionality

#### Adding email alerts for content published and displayed in your Specialist Publisher Finder

When your Finder is live, ask the GDS team to set up alerts based on the filters in your Finder.

Example can be seen here when selecting ‘Get emails’ https://www.gov.uk/raib-reports

#### Link from your Specialist Publisher to another page on GOV.UK

If you are linking to your Finder from another page on GOV.UK (say an Organisation page) you might want users to be able to return to that page from the Finder. Once your Finder is live, ask the GDS team to add the link to your Finder.

eg https://www.gov.uk/raib-reports with the link ‘From Rail Accident Investigation Branch’)
