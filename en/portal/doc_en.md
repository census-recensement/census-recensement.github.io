## Data Dictionary

The CCDDP census inventory consists of a custom set of metadata fields described in this data dictionary. Each inventoried item has a parallel metadata record in both the English and the French inventories. The inventories are searchable through our proof-of-concept portal, and can be downloaded from Borealis (link).

For more information about the CCDDP project goals and scope, see the project website and the project documentation on Borealis (link).

## Field descriptions

### Title

#### Definition:

The title of the census item

#### Notes:

- If no title was included on the census item, the cataloguer created one and enclosed it in square brackets.

- If the item was only published in one official language, a title in the other official language was not created. In the result set for the other official language, the title will appear as published, with a note in square brackets “[English only]” or “[Français seulement]”.

#### Values:

text field

---

### Content type

#### Definition:

The type of content in the census item

#### Values:

- Aggregate data tables. Statistical tables that summarize census data.

- Analytical reports. Reports that analyze census data. While these may include items of other content type within them (data tables etc), these are generally not inventoried separately.

- Census reference products. Documentation and informational products. 

- Census returns. Original archived census records. These are included in the CCDDP inventory if they are available in a searchable or downloadable database form. 

- Digital spatial products. Geospatial boundary files and other geospatial data.

- Geographic reference products. This includes documentation and informational products related to spatial data and maps, as well as attribute information products (such as correspondence files, GeoSuite, etc).  

- Microdata. Anonymized individual-level data. This includes Public Use Microdata Files (PUMFs) produced by Statistics Canada as well as microdata files produced by the research community.

- Monographs. Book-length analysis on census subjects.

- Product level documentation. Documentation created specifically to guide in the use of one particular item.

- Reference maps. Maps showing census geographic boundaries

- Technical reports. Reports that describe methodology and other technical details around the collection of census data and production of census products.

- Thematic maps. Maps showing census themes.

---

### Supplementary

#### Definition:

Flag to indicate that the item was not published by an official census data authority as part of a census release. The material may consist of additional data, converted formats, or supplementary documentation created to assist in the use of official material.

Notes: Data products created at a later date using census records or publications, such as microdata files (created from archival census returns), and spatial boundary files (created from reference maps) are note considered supplementary; these are core in-scope materials. 

#### Values:

Y/N binary, where Y indicates that the item is supplementary

---

### Census year (of publication)

#### Definition:

The census the item was published with, tracked by the year the census was conducted.

#### Notes:
 

Only one year can be stored in this field. If the item was not published “with” a census (it is supplementary or published after the fact) this field is left blank.

#### Values:

Please consult the list of census years (link) for a complete list of the censuses included in the inventory.

---

### Census Year(s) covered by item

#### Definition:

All censuses that the item covers, tracked by the years the censuses were conducted.

#### Notes:

Multiple census years can be stored in this field. For example, if a data table contains comparative data for three censuses, each of them will be tagged here.

#### Values:
 

Please consult the list of census years (link) for a complete list of the censuses included in the inventory.

---

### ID

#### Definition:

A unique identifier for the census item.

#### Values:

Alphanumeric unique identifiers

---

### Parallel Title

#### Definition:

The title in the alternate official language.

#### Values:

text field

---

### Author/Producer of Item

#### Definition:

The person or entity responsible for producing the census item. 

#### Values:

Please consult the list of authors/producers (link) for a complete list of the authors/producers included in the inventory.

---

### Subject

#### Definition:
 

The subject matter of the census item.

#### Notes:
 

Subjects are selected from an authority list created and maintained by the CCDDP project team. 

#### Values:

Please consult the subjects authority list (link).

---

### Release date

#### Definition:
 

The year the item was published or released.

#### Notes:
 

This is distinct from the “census year” which is the year the census was conducted. If the publication year is not know, this field is left blank.

#### Values:

text field

---

### Geographic coverage

#### Definition:

The overall geographic area that is covered by the item.

#### Notes:

This field uses the terminology that was used to describe regions at the time of the census. When terminology used in the census is inconsistent with official names at the time, both terms are tagged. The geographic coverage authority list contains some information about the range of years that apply for each colonial territory and current province/territory.

#### Values:

Please consult the geographic coverage authority list (link).

---

### Geographic units

#### Definition:

The specific geographic units the data is broken down by.

#### Notes:

This field uses the terminology indicated on the item itself, even when that terminology differs from contemporary usage. The geographic units authority list provides some information about the range of years that apply for each geographic unit name.

#### Values:

Please consult the geographic units authority list (link).

---

### Language

#### Definition:

The language(s) of the item

#### Values:

- English

- French

---

### Found in (print volume)

#### Definition:

The volume the item is found within.

#### Notes:

This field is completed for born-print items only and is completed only for items that are part of a larger volume. 

#### Values:

Please consult the publications list (link).

---

### Found in (digital file)

#### Definition:

The filename and/or number of the particular file that this item is found within

#### Notes:

This field is only used in cases where multiple separate tables (with their own table numbers) were released within a single computer file.

#### Values:

text field

---

### Page numbers (born print only)

#### Definition:

The page numbers where the item can be found.

#### Values:

text field

---

### Table series (born digital only)

#### Definition:

The name of the series the item is associated with

#### Notes:

This field is used for the series names that Statistics Canada has used to organized digital data tables since the 1960s when digital tables were first released.

#### Values: (update this when inventory is complete)

- Basic summary tabulations

- Data tables

- Dimension series

- Focus on Geography series

- Highlight tables

- Nation series

- Profile series

- Topic-based Tabulation

- User summary tapes

---

### Product Identifier

#### Definition:

The official Statistics Canada/Government of Canada product ID number (if applicable).

#### Values:

text field

---

### Format

#### Definition:

The physical or digital file format(s) the item is available in.

#### Notes:
 

Multiple selections are allowed.

#### Values: (update this when inventory is completed)

- ASCII text

- CSV

- DOC

- DTA

- IVT

- JPG

- JP2

- MDB

- Microform

- PDF

- Print

- Print XML

- SAV

- TAB

- TXT

- Website

- XLS

- XML

---

### Coordinate system

#### Definition:
 

Coordinate system information (applies for maps and spatial data)

#### Notes:

This information may not be known and so may not be completed for all maps & spatial data.

#### Values:
 

text field

---

### Data Access

#### Definition:
 

URL(s) for accessing the item.

#### Values:

text field

---

### Related Materials & Documentation

#### Definition:
 

Links to other related items in the inventory.

#### Values:
 

titles of items included in the inventory database

---

### ID-F (ID-E in the French inventory)

#### Definition:

ID of the census items in its alternate language

#### Values:
 

text field

---

### Digitization/data quality

#### Definition:

Indication of the data quality for digitized, born-print items.

#### Notes:
 

From the four possible values, two are selected in each instance: complete/incomplete, and high/low quality.

#### Values:

- Complete

- Incomplete

- High quality

- Low quality

---

### Data access notes

#### Definition:

Notes related to accessing & using the item.

#### Values:

text field

---

### Additional notes

#### Definition:

Any other relevant notes about the item

#### Values:

text field