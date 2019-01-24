**NCDHC Feeding Status Observation Profile**

This profile sets minimum expectations for the [Observation] resource to record, search and fetch feeding status associated with the baby patient. It identifies which core elements, extensions, vocabularies and value sets **SHALL** be present in the resource when using this profile. The profile is at draft stage and under review by the Child Health Working Group. 

**Example Usage Scenarios:**

The following are example usage scenarios for the National Child Digital Health interactions
profile:

-   Query for Feeding Status of the baby patient
-   Record Feeding Status of the baby patient

##### Mandatory Data Elements and Terminology


The following data-elements are mandatory (i.e data MUST be present). These are presented below in a simple human-readable explanation. Profile specific guidance and examples are provided as well.  The [**Formal Profile Definition**](#profile) below provides the  formal summary, definitions, and  terminology requirements.  

**Each Observation must have:**

1.  a status  
1.  a LOINC and SNOMED code which tells you what was recorded and is taken from the “LOINC Code” & "SNOMED CT" columns respectively in the table below.
1.  a subject (Patient)
1.  a time indicating when the details was recorded
1.	a performer detailing who has recorded the details.
1.  a CodableConcept representation of the feeding status reported. Applicable types are defined in the ValueSet: http://hl7.org/fhir/ValueSet/newborn-feeding-status
    

**Profile specific implementation guidance:**

* To be added



---

<table class="grid">
  <thead>
    <tr>
      <th>Observation</th>
      <th>LOINC Code</th>
      <th><em>LOINC Name </em>and Comments</th>
	  <th>SNOMED Code</th>
      <th><em>SNOMED Name </em>and Comments</th>      
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Feeding Status</td>
      <td>P72581-9</td>
      <td>Feeding and dietary status</td>
      <td>129007004</td>
	  <td>Feeding</td>	  
    </tr>    
  </tbody>
</table>

---


#### Examples

- [Feeding Status](Observation-feeding-status.html)

[Observation]: http://hl7.org/fhir/observation.html
[extensible]: http://hl7.org/fhir/terminologies.html#extensible
[General Guidance Section]: definitions.html