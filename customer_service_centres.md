## Customer service centres 0.1

Customer service centres are places where citizens go to pay fees (rates, fines, pet registration), deposit planning applications, or otherwise interact with council services.


####General recommendations:

* Format: Point data. CSV (preferred), GeoJSON, Shapefile
* Dataset name: [Council name] customer service centres
* data.gov.au tag: `opencouncildata-customer-service-centres-0.1`

#### Required fields

* `lat`: latitude
* `lon`: longitude

#### Recommended fields

* `name`: A name identifying the centre. E.g. "Preston Customer Service Centre"
* `services`: Comma-separated list of services provided by the centre. For example: "pet registration,parking fines,rates". Possible values include:
  * `pet registration`
  * `parking fines`
  * `rates`
  * `planning`
  * `building permits`
  * (add your own, please provide feedback)
* `address`: Street address. E.g. "274 Gower Street, Preston, VIC 3072"

* `languages`: Comma separated list of non-English languages spoken at the centre (or provided by phone interpreter), in ISO 639-1 (two-letter) codes. For example: `it,vi,zh`
* `accessible`: Free text description of accessibility. For example: "Fully accessible to wheelchair users; disabled parking at front."
* `monday`: normal opening hours on Mondays, in 24 hour `HH:MM-HH:MM` format. For example: `08:00-17:30`.
* `tuesday`: as above.
* `wednesday`: as above.
* `thursday`: as above.
* `friday`: as above.
* `saturday`: as above.
* `sunday`: as above.
* `holiday`: normal opening hours on public holidays.

#### Optional fields
* `description`: Free text description of services or other information.
* `phone`: Telephone number of this center, if any.