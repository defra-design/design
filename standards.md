## Defra Interaction design standards

Interaction designers determine the best way for users to interact with services, from the overall flow/user journey to individual design elements. 

More information on [what Interaction Designers do](/interaction-design.md).

## Prototyping
A prototype should be the quickest, simplest way to learn about something, or to test an idea.


### Versioning

### Documentation


## Design patterns

Design patterns solve the common problems so teams can focus on the things uniques to their service and it’s users.

Check the [GOV.UK Design System](https://design-system.service.gov.uk/) to see if the component or pattern you need is already being used across government.

If you cannot find what you need in the GOV.UK Design System you can:

* [see if it is being worked on by other teams across government and add your findings](https://design-system.service.gov.uk/community/backlog/)
* see if it is being worked on by someone in [Defra](https://github.com/DEFRA/design-system-backlog/issues) and add your findings 
* propose a new pattern in [Defra](https://github.com/DEFRA/design-system-backlog/issues)
* [propose a new pattern in the cross gov design system](https://design-system.service.gov.uk/community/propose-a-component-or-pattern/)

All patterns must be [useful and unique](https://design-system.service.gov.uk/community/contribution-criteria/#new-proposals).

<!-- ### Iterating a design pattern
Existing design patterns can be used as starting points but may need to be iterated to suit the needs of users of a particular service. 

To do this add a class to the component with a Defra namespace.

```
<button type="submit" class="govuk-button">
  Save and continue
</button>
```

```
<button type="submit" class="govuk-button defra-button">
  Save and continue
</button>
``` -->
### Creating new a design pattern
 
To create a new pattern use a Defra namespace to avoid issues with CSS inheritance.

```
<header role=“banner” class=“defra-internal-header”>
   <div class=“defra-logo”>
       <a href=“https://www.gov.uk/government/organisations/department-for-environment-food-rural-affairs” title=“Go to the Defra Design Library homepage” class=“defra-logo__link”>
           <span class=“c-defra-logo__title”> Defra </span>
       </a>
   </div>

   <div class=“defra-internal-service-name”>
       <a href=“/” title=“Go to the homepage” class=“defra-internal-service-name__link”>
         Design resources for Defra
       </a>
   </div>
</header>
```

