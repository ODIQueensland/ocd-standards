## Building accessibility ratings 1.1

Some councils provide ratings on accessibility of buildings for wheelchair users. These ratings are in high demand by certain community groups wanting to choose venues suitable for all their members. These ratings may be available for only council buildings, or more broadly.

There are no known standards for this kind of data, and some councils combine them in different ways (eg, a rating of 0, 1 or 2 for the building as a whole).

####General recommendations:

&nbsp;| Recommendation
------|------------
Format| CSV (preferred), Shapefile, GeoJSON
Dataset name| [Council name] Building Accessibility Ratings
data.gov.au tag| `building-accessibility`, `opencouncildata`, `ocd-building-accessibility-1.1`

#### Required fields

Field | Description
------|------------
`lat`, `lon`| Latitude, longitude, decimal degrees of centroid or entrance to building. (EPSG:4326)

#### Recommended fields
Field | Description
------|------------
`entrance`| Access into the building and its main services.<br/> `yes`: an unpowered, wheelchair user can enter the building and access public services without assistance<br/>`assisted`: a wheelchair user can enter the building if assisted. _For example, a steep ramp, or a lift requiring an authorised operator._<br/>`no`: there is limited or no access for wheelchair users. _For example, a cinema with a ramp entrance, but steps to individual theatres._
`parking`| `yes`: disabled parking spaces are available<br/> `no`: there is no designated disabled parking
`toilets`| `yes`: toilets suitable for wheelchair users are available<br/>`no`: there are no toilets suitable for use by wheelchair users
`name`| A name identifying the building, organisation or business name.
`address`| The building's street address.

#### Optional fields
Field | Description
------|------------
`id`| A council-specific identifier that can used to link to other council-published data for that building, such as a building footprint.
`assessed`| Date of most recent accessibility assessment, in ISO 8601 (YYYY-MM-DD).
`comment`| Text description supplementing the `entrance`,`parking` and `toilets` fields.

