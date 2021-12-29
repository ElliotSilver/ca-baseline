# CA Core DiagnosticReport (Note) Profile
<div xmlns="http://www.w3.org/1999/xhtml" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
	<blockquote class="stu-note">
		<p> This profile initially put forth placeholders for the value sets used in category and code. Further work is required to determine if this profile should align to the value set in use in US Core (https://www.hl7.org/fhir/us/core/ValueSet-us-core-diagnosticreport-category.html and https://www.hl7.org/fhir/us/core/ValueSet-us-core-diagnosticreport-report-and-note-codes.html) or if a Canadian value set needs to be created.
    <br>
	</blockquote>
  </div>

This profile sets minimum expectations to support collection of diagnostic report information for reports and notes. Generated as a first step toward creating a set of Canadian Baseline FHIR profiles. It identifies which core elements, constraints and value sets SHALL be present in the resource instance when using this profile.

This profile defines core localisation concepts for use in an Canadian context.

## Mandatory Data Elements
All elements or attributes defined in FHIR have cardinality as part of their definition - a minimum number of required appearances and a maximum number.

Most elements in FHIR specification have a minimum cardinality of **0**, which means that they may be missing from a resource when it is exchanged between systems.

**Required elements:**
* status of the diagnostic report
* category of the diagnostic report
* code that describes the diagnostic report
* subject of the report
* time when report was created

## Must Support Data Elements
Some elements are labeled as MustSupport meaning that implementations that produce or consume resources SHALL provide "support" for the element in some meaningful way (see [Must Support](https://build.fhir.org/ig/HL7-Canada/ca-baseline/general-guidance.html#must-support) definition).

Following elements are marked as Must Support in the Canadian DiagnosticReport Note profile to aid record matching in databases.

**Must Support elements:**
* status of the report
* category that classifies the report
* code that describes the diagnostic report
* subject of the report
* healthcare event this report is about
* time when report was created
* time when report was issued
* diagnostic service responsible for report
* Media that are part of this report
* Attachments that are part of this report

## Usage Note
