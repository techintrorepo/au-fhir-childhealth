**NCDHC Method Of Delivery Observation Profile**

This profile sets minimum expectations for the [Observation] resource to record, search and fetch Birth Type associated with the baby patient. It identifies which core elements, extensions, vocabularies and value sets **SHALL** be present in the resource when using this profile.

**Example Usage Scenarios:**

The following are example usage scenarios for the National Child Digital Health interactions
profile:

-   Query for Birth Type of the baby patient
-   Record Birth Type of the baby patient

##### Mandatory Data Elements and Terminology


The following data-elements are mandatory (i.e data MUST be present). These are presented below in a simple human-readable explanation. Profile specific guidance and examples are provided as well.  The [**Formal Profile Definition**](#profile) below provides the  formal summary, definitions, and  terminology requirements.  

**Each Observation must have:**

1.  a status  
1.  a LOINC and SNOMED code which tells you what was recorded and is taken from the “LOINC Code” & "SNOMED CT" columns respectively in the table below.
1.  a subject (Patient)
1.  a time indicating when the details was recorded
1.	a performer detailing who has recorded the details.
1.  a CodableConcept representation of the Types reported. Applicable types are defined in the ValueSet: http://hl7.org.au/fhir/ch/ValueSet/type-of-birth-snomed
    

**Profile specific implementation guidance:**

* To be added



---

<table class="grid">
  <thead>
    <tr>
      <th>Labour and Delivery</th>
      <th>LOINC Code</th>
      <th><em>LOINC Name </em>and Comments</th>
	  <th>SNOMED Code</th>
      <th><em>SNOMED Name </em>and Comments</th>      
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Birth Type</td>
      <td>72149-8</td>
      <td>Delivery method [RHEA]</td>
      <td>289258004</td>
	  <td>Finding of pattern of delivery</td>	  
    </tr>    
  </tbody>
</table>

---


#### Examples

- [Birth Type](Observation-method-of-delivery.html)

[Observation]: http://hl7.org/fhir/observation.html
[extensible]: http://hl7.org/fhir/terminologies.html#extensible
[General Guidance Section]: definitions.html