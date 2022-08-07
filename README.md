# Credential Engine, 1EdTech, PESC, HR Open Standards, Schema.org, CEDS Files for T3 DESM Testing

During testing of the DESM tool, a consistent set of well-formed schemas from established  Data Standards Organizations (DSOs) including Credential Engine, HR Open Standards, PESC, CEDS, Credential Engine, Schema.org, ASN and 1TechEd.  Test data (schemas and concept schemes) for testing have been gathered together in GigHub. These test files cover the major forms that data needing to be ingested into the DESM tool will take including XML (XML Schema), CSV, JSON (JSON Schema), and RDF (RDF Schema) via its common serializations including RDF/XML, JSON-LD, RDF/JSON (resource-centric) and Turtle.

This README documents the location of those well-formed schemas to be used in testing.  Some of the schemas are quite large including those of Schema.org, PESC, HR Open and Credential Engine, ASN, CEDS. The large size of these schemas is the result of their covering multiple classes in single files. While there are use cases where a large number of DSOs will be mapping a large number of classes, the more likely general use case for DESM will be crosswalking a limited number of DSO schemas describing a limited number of classes. Where the number of classes being crosswalked is small, large schemas in which they may be embedded may be right-sized, by extracting only the classes and associated properties needed for the crosswalking task prior to loading the abbreviated schema into the DESM instance. As a result, most schema loads will be relatively constrained in size. 

The schema files needed for the T3 DESM mapping from Credential Engine, 1EdTech, PESC, HR Open Standards, Schema.org, UW/D2L are listed below along with URLs where the files have to be accessed outside the repo.

### CEDS—Common Education Data Standards
The CEDS schema is published periodically in a large CSV file. Since any single use case of the DESM tool is unlikely to need even a fraction of this large CSV set, the file can be edited down to only the applicable data before uploading in the DESM tool.
* Version 9 CEDS CSV (Spreadsheet): https://github.com/stuartasutton/desmSchemas/blob/main/CEDS/CEDS-V9-with-Extend.xlsx

### Credential Engine
TCredential Engine maintains three namespace schemas—CTDL, CTDL-ASN and QData. All three namespace schemas are in continuous continuous development and are not episodically published in versions. As a result, the three namespace and select concept schemes here in GitHub should be access for DESM upload from their source on the Credential Engine website. Each of the three namspaces comes in two flavors: (1) with meta tags, and (2) without meta tags. The "without meta tags" flavor is the most common form while the "with meta tags" is the most useful to downstream systems using the schemas. For DESM testing purposes, both flavors should be tested. The DESM's filtering should simply ignore the meta tags from the http://credreg.net/meta/terms/ namespace. 

<ul>
   <li>CTDL: Primary namespace (<em>Serializations Homepage:</em> https://credreg.net/ctdl/schema)
      <ul>
         <li>With Meta Tags: https://credreg.net/ctdl/schema/encoding/json</li>
         <li>Without Meta Tags: https://credreg.net/ctdl/schema/encoding/json?includemetaproperties=false</li>
      </ul></li>
   <li>CTDL-ASN: Competency Framework namespace (<em>Serializations Homepage:</em> https://credreg.net/ctdlasn/schema)
      <ul>
         <li>With Meta Tags: https://credreg.net/ctdlasn/schema/encoding/json</li>
         <li>Without Meta Tags: https://credreg.net/ctdlasn/schema/encoding/json?includemetaproperties=false</li>
      </ul></li>   
   <li>QData Quantitative Data namespace (<em>Serializations Homepage:</em> https://credreg.net/qdata/schema)
      <ul>
         <li>With Meta Tags: https://credreg.net/qdata/schema/encoding/json</li>
         <li>Without Meta Tags: https://credreg.net/qdata/schema/encoding/json?includemetaproperties=false</li>
      </ul></li>  
</ul>

**Note:** All three namespace schemas include all relevant concept schemes and concepts encoded using W3C's Simple Knowledge Organization System (SKOS); <u>however</u> each concept scheme is also published separately. The separately published concept schemes are available through the left-hand selection panel on each namespace serialization homepage:  
<ul>
   <li>CTDL, 26 concept schemes</li>
   <li>CTDL-ASN, 1 concept scheme</li>
   <li>QData, 6 concept schemes</li>
</ul>

### 1EdTech (<em>previously IMS Global</em>)
The IMS Gloab (1EdTech) folder contains JSON schemas for a number of classes including Comprehensive Learner Record (CLR), Course, Organization, and CASE (competency frameworks). The CASE file comes in both JSON and JSON-LD.

### PESC—Postsecondary Electronic Standards Council
There are two PESC schemas (XML Schema) for testing, Academic Record (Academic_Record_v_1.13.xsd) and Core Main (CoreMain_v_1.19.xsd). Each of these files make references to the other.

### HR Open Standards
HR Standards is the largest (most complex) JSON data standard covering all of the human resource domain. It's GitHub folder here contains a good deal of it, but certainly not all. The XSD files contain both classes and properties, but also enumerations and tagging files.

There is Google sheet that identifies where the XSD files in this GitHub folder show up in teh description of select major classes (Course, Competency, Organization etc.): https://docs.google.com/spreadsheets/d/1yXQDO5m3GalqF_ylyYUvJo7DO47dXocVhj7JiedGVSM/edit#gid=457410372. The files in the Google sheet shaded blue and with the words "CodeList" in their names define concept schemes/enumerations.

### Schema.org
The Schema.org schema is very large. It is modeled in RDF and expressed in a number of serializations including JSON-LD, RDF/XML, Turtle, CSV, Triples and Quads. URL's to four of these serializations are listed below:

* JSON-LD: https://schema.org/version/latest/schemaorg-current-https.jsonld
* RDF/XML: https://schema.org/version/latest/schemaorg-current-https.rdf
* Turtle: https://schema.org/version/latest/schemaorg-current-https.ttl
* CSV: https://schema.org/version/latest/schemaorg-current-https-types.csv

### UW/D2L (ASN)

The ASN schemas and concept schemes to use with the DESM tool are maintained in a separate github repo: [https://github.com/stuartasutton/asn](https://github.com/stuartasutton/asn)
