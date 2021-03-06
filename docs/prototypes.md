###### [Portable Linked Profiles](http://hackers4peace.net/plp)

# Prototypes

## About

The family of Portable Linked Profiles Services is built around a modular microservice architecture. Everything has its place, so it doesn't need to be doubled, if it merely can be referenced.

The Prototypes define the general data models used with Portable Linked Profiles.

## Source

The source code can be found at

> https://github.com/hackers4peace/plp-prototypes

## Types

### Person

* status *implementing*
* schemas
 * [x] http://schema.org/Person
 * [ ] http://smiy.sourceforge.net/cco/spec/cognitivecharacteristics.html
 * [ ] http://microformats.org/wiki/h-card
 * [ ] http://microformats.org/wiki/h-resume

http://profiles.open-steps.org/provider/7ce5f07a-1c3c-4e35-90c9-e51bce25e04a
```json
{
  "name": "Alex Corbi",
  "description": "Software developer based in Berlin since 2009. Co-Founder of the independent initiative Open Steps: A journey around the world discovering and showcasing Open Knowledge projects.",
  "website": "http://www.open-steps.org",
  "address": [
    {
      "city": "Berlin",
      "country": "Germany"
    }
  ],
  "memberOf": [
    {
      "name": "Open Steps"
    }
  ],
  "contactPoint": [
    {
      "type": "Email",
      "id": "alex@open-steps.org"
    },
    {
      "type": "Github",
      "id": "http://github.com/opensteps"
    },
    {
      "type": "Twitter",
      "id": "http://www.twitter.com/acorbi"
    }
  ],
  "interest": [
    {
      "name": "Open Data"
    },
    {
      "name": "Open Source"
    },
    {
      "name": "Software Development"
    },
    {
      "name": "Data Visualisation"
    }
  ],
  "@id": "http://profiles.open-steps.org/provider/7ce5f07a-1c3c-4e35-90c9-e51bce25e04a",
  "@type": "Person",
  "@context": "http://plp.hackers4peace.net/context.jsonld"
}
```

### Organization

* status *implementing*
* schemas
 * [x] http://schema.org/Organization
 * [ ] http://microformats.org/wiki/h-card

Example

http://profiles.open-steps.org/provider/30fa6739-6440-45cf-abd5-e6d1c8810ece
```json
{
  "name": "Aberdeen City Council",
  "description": "The Local Authority for the Aberdeen City geographic region",
  "telephone": "01224 522000",
  "website": "http://www.aberdeencity.gov.uk",
  "logo": "http://www.aberdeencity.gov.uk/web/Templates/acc-home-2011_files/acc-logo.gif",
  "address": [
  {
    "street": "Marischal College, Broad Street",
    "code": "AB10 1Ab",
    "city": "Aberdeen",
    "country": "UK"
  }
  ],
  "member": [
  {
    "name": "ian Watt",
    "jobtitle": "e-Government Manager",
    "description": ""
  }
  ],
  "contactPoint": [
  {
    "type": "Email",
    "id": "webmonitor@aberdeencity.gov.uk"
    },
    {
      "type": "Twitter",
      "id": "@aberdeencc"
    }
    ],
    "interest": [
    {
      "name": "Open Data"
      },
      {
        "name": "GIS"
      }
      ],
      "@type": "Organization",
      "@id": "http://profiles.open-steps.org/provider/30fa6739-6440-45cf-abd5-e6d1c8810ece"
    }
```

### Event

* status *implementing*
* schemas
 * [x] http://schema.org/Event
 * [ ] http://microformats.org/wiki/h-event

Example
```json
{
  "name": "OK Lab Berlin",
  "description": "Regular Hacknight for the OK Lab Berlin members. Please join us if you are already working on a project. New members are warmly welcomed on every second Monday of the month to our open meet ups. ",
  "url": "http://www.meetup.com/OK-Lab-Berlin/",
  "image": "",
  "startDate": "19/01/2015 19:00",
  "endDate": "19/01/2015 24:00",
  "organizer": [
    {
      "name": "Code For Germany",
      "website": "http://www.codefor.de"
    }
  ],
  "performer": [],
  "eventStatus": "Scheduled",
  "location": [
    {
      "street": "Tempelhofer Ufer 23/24",
      "code": "10963",
      "city": "Berlin",
      "country": "Germany"
    }
  ],
  "workPerformed": [
    {
      "name": "PLP: Portable Linked Profiles",
      "url": "http://profiles.allmende.io"
    }
  ],
  "@type": "Event",
  "@context": "http://plp.hackers4peace.net/context.jsonld"
}
```
### Place

* status *implementing*
* schemas
 * [x] http://schema.org/Place
 * [ ] http://microformats.org/wiki/h-geo

Example
```json
{
  "name": "Wikimedia Deutschland",
  "description": "Wikimedia ist eine internationale gemeinnützige Organisation, die Freies Wissen fördert. Durch die Sammlung, Entwicklung und Verbreitung von Freien Inhalten in allen Sprachen der Welt wird dieses Ziel verfolgt. Wikimedia Deutschland - Gesellschaft zur Förderung Freien Wissens e.V. unterstützt verschiedene Projekte. Das größte ist Wikipedia - die freie Enzyklopädie, deren Betreiberin die Wikimedia Foundation ist.",
  "telephone": "+49 (0)30-219 158 26-0 ",
  "url": "https://wikimedia.de/wiki/Kontakt",
  "image": "https://www.wikimedia.de/w/images.homepage/c/c9/Logo.png",
  "address": [
    {
      "street": "Tempelhofer Ufer 23/24",
      "code": "10963",
      "city": "Berlin",
      "country": "Germany"
    }
  ],
  "event": [],
  "@type": "Place",
  "@context": "http://plp.hackers4peace.net/context.jsonld"
}
```
### Project

 * status *implementing*
 * schemas
 * [x] http://schema.org/CreativeWork

Example
```json
{
  "name": "PLP: Portable Linked Profiles",
  "description": "PLP proposes a pattern for the creation, storage, listing and representation of public profile data for people, groups, organizations, venues and a large etcetera. Based on Open Web Standards, Common Vocabularies and Open Source technologies, it offers users the possibility to own the their data diverging from current mainstream and centralized profile platforms.",
  "url": "https://github.com/hackers4peace/plp-docs",
  "image": "http://codefor.de/assets/projects/berlin/portablelinkedprofiles.png",
  "version": "0.1",
  "license": "http://unlicense.org/",
  "copyrightHolder": {
    "name": "",
    "url": ""
  },
  "contributor": [
    {
      "name": "Elf Pavlik",
      "website": "http://elf-pavlik.wwelves.org/"
    },
    {
      "name": "Alex Corbi",
      "website": "http://www.open-steps.org"
    },
    {
      "name": "Jon Richter",
      "website": "http://allmende.io/"
    },
    {
      "name": "Lynn Foster",
      "website": "http://mikorizal.org/"
    },
    {
      "name": "Tibor Katelbach",
      "website": "http://www.pixelhumain.com/"
    }
  ],
  "discussionUrl": [
    {
      "url": "http://profiles.allmende.io/"
    },
    {
      "url": "http://directory.open-steps.org/"
    },
    {
      "url": "https://github.com/hackers4peace/plp-docs"
    }
  ],
  "isPartOf": [],
  "workExample": [],
  "workPerformed": [],
  "@type": "Project",
  "@context": "http://plp.hackers4peace.net/context.jsonld"
}
```

### Asset

* status *planned*
* schemas
 * [ ] http://schema.org/Product
 * [ ] http://schema.org/Service
 * [ ] http://microformats.org/wiki/h-product
