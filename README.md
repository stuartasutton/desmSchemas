# Credential Engine, 1EdTech, PESC, HR Open Standards, Schema.org, CEDS Files for T3 DESM Testing

The schema files needed for the T3 DESM mapping from Credential Engine, 1EdTech, PESC, HR Open Standards, Schema.org, UW/D2L

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

**Note:** All three namespace schemas include all relevant concept schemes and concepts encoded using W3C's Simple Knowledge Organization System (SKOS); <u>however</u> each concept scheme is also published separately. The separately published concept schemes are available through the left-hand selection panel on each serialization homepage:  
<ul>
   <li>CTDL, 26 concept schemes</li>
   <li>CTDL-ASN, 1 concept scheme</li>
   <li>QData, 6 concept schemes</li>
</ul>

### 1EdTech

### PESC

### HR Open Standards

### UW/D2L (ASN)

The ASN schemas and concept schemes are maintained in a separate github repo: [https://github.com/stuartasutton/asn](https://github.com/stuartasutton/asn)
