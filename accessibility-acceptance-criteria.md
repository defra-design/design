<!-- Nav -->
* [Interaction design and service design](/README.md)
* [What interaction designers and service designers do](/design.md)
* [Defra Design community](/community.md)
* [Tools and resources](/tools-and-resources.md)
* [Defra design standards](https://github.com/DEFRA/design-standards)
* [Specialist Publisher](/specialist-publisher.md)
* Accessibility acceptance criteria
* [Design crits](/design-crits.md)
* [Case studies](/case-studies.md)

# Accessibility acceptance criteria

Ensuring a service is accessible is often something that a team decides to do either prior to a service assessment or when it deems the service is ready for release. A better way to do it is to make it part of the acceptance criteria for every sprint. This not only ensures that the team doesn’t get any nasty surprises but is a way for a team to work effectively together by ensuring the acceptance criteria by which they deliver code is aligned with accessibility requirements.

Using the latest version of the GOV.UK Design System ensures a lot of things are baked in, but sometimes there are different patterns and components especially with internal and case management system.

### General

* Actionable with keyboard or touch or mouse or voice
* Check using assistive technologies. Tested with at least one screen reader
* Zoom page to 200%, then 400% - is content still legible? Test on all major browsers
* Try without css – does content make sense and appear in a logical order?
* Test without javascript – does content make sense and appear in a logical order?
* View on variety of screen sizes
* Used with high contrast mode
* Invert colours (eg white on black)
* Test with voice dictation (eg Voiceover on Mac)
* Appearance changes on interaction
* Links should look like links
* Suitable vertical spacing between lines and paragraphs
* Avoid italics, block capitals or justified text
* Text can be resized
* Check html mark-up is valid
* Check in a range of browsers and devices

### Specific

* Check that headings and lists are used correctly
* Use the https://accessibility-bookmarklets.org/install.html to verify that all content is in a landmark and that the correct landmarks are used in the correct places.
* Use bookmarklet to ensure text spacing meets WCAG 1.4.12
* Colour contrast testing. Perhaps not a full test, but focusing on colour combinations that look suspect. This needs to include hover and focus states and needs to be done on all various responsive layouts (a colour contrast of at least 4.5:1 between text and the background)
* Where there is a service that includes images, test the service without images being displayed. This is not a WCAG requirement, but it is a GDS requirement. Many techniques that provide alternate text for assistive technologies (such as aria-label attributes and hidden text) do not provide visible text for sighted users when images are not displayed
* For each page built or updated as part of the sprint, use the HTML validator at https://validator.w3.org/nu/ and use https://dotjay.github.io/wcag-parsing-filter/bookmarklet/ to filter the results so that only WCAG non-compliances are shown
* No timeout unless as a security precaution
* Download links labels include file format and size
* Only use tables to present data
* Don’t communicate using colour alone
* All form inputs have labels

### Content

* Using plain English
* Explain unusual words and jargon
* Most important information at the start
* Logically structured, using sub-heads, bullets and short sentences
* Consistent use of formatting (eg H1/H2 etc)
* Each page has unique, descriptive h1 and page title
* Content written in a task focused way
* Default text size that is comfortable to read
* Headings, links and button text must be unique and descriptive
* Alt tags, captions and image descriptions for images
* Link text that is descriptive (eg: Read our [Privacy Policy])
* (Where relevant) transcripts for any audio and/or video content
* If there are documents as attachments ensure they are accessible (eg PDFs to be accessible – https://www.gov.uk/guidance/how-to-publish-on-gov-uk/accessible-pdfs)
* Where relevant, think about provision of alternative formats (eg easy read format)
* Error messages suggest ways to fix error
* Error messages should show a summary of errors above the h1 and move focus to it
* Error message summary should include an h1 message that tells the screen reader user there is a problem, and gives a list of descriptive errors with links to the relevant fields

### Reference and furhter reading

* Unsorted collection of accessibility acceptance criteria https://alphagov.github.io/a11y-dev-workshop/criteria
* ARIA documentation: https://w3c.github.io/using-aria/#ariachecklist
* Paciello Group: https://developer.paciellogroup.com/blog/2014/09/web-components-punch-list/
* Improving accessibility with accessibility acceptance criteria https://insidegovuk.blog.gov.uk/2018/01/24/improving-accessibility-with-accessibility-acceptance-criteria/
