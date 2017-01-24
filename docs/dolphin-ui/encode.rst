*******************************
Dolphin ENCODE Submission Guide
*******************************

Getting Started
===============

Not everyone can submit to ENCODE, you must first have contact with the ENCODE Consortium before considering to design,
create, and analyze a projet that you are willing to submit to ENCODE.  Please visit the `ENCODE website`_ for more details
on ENCODE.  Not all that apply will be able to submit to ENCODE.

.. _ENCODE website: https://www.encodeproject.org/

Meta-data Collection/Input
==========================

Assuming you are to submit to ENCODE, you are going to want to collect a various amount of meta-data that surrounds your project.
This is a cruicial step in submitting to encode and without the proper meta-data for submission submission will not be possible.

As a curator for your experiment, you are going to want to collect meta-data from all stages of the experiment.  This includes:

	* Protocol information within the wet lab
	* Sequencer and sequencing information
	* Analysis programs and versions used
	* Outline/Goal of your analysis process
	
These bullet points encompass a large amount of information, however if you keep proper track of all of this information, this will make
submission to ENCODE a smooth process.

More information about which fields are required and which fields you should consider keeping track of can be found at the ENCODE website listed
above.  Addition information can be found by contacting someone from ENCODE directly, or by keeping in contact with your assigned data wrangler.

ENCODE Submission Process
=========================

*The Breakdown*

In order for ENCODE to retain the information you wish to send them, it must be passed to their servers using JSON objects.  A JSON object
is a form of organizing data that is easy to read and to create.  Encode stores information passed by users within linked json objects using aliases,
uuids, and accession numbers.

You will be passing JSON objects created from the meta-data you have gathered and input into the Dolphin system in order to represent your experiment and
the files you will be sending to encode.

*The Detailed Version*

There are 2 major submission phases that include mutliple sub-steps along the way.  The first phase we shall call the 'overall meta-data submission' step.
For this phase, you will be submitting meta-data that encompasses your overall experiment.  For this, we submit 7 specific JSON objects in a specific order:

	* Donor JSON
	* Experiment JSON
	* Treatment JSON
	* Biosample JSON
	* Library JSON
	* Antibody JSON
	* Replicate JSON
	
We submit these JSON objects from top to bottom due to the fact that some of the JSONs require the accession number or alias of a previous step.  Without this
unique identifier, the JSONs cannot be properly linked and will thus not be correct.

Once the overall meta-data step has completed successfully, you can then enter the 'file data' submission phase.  During this phase you will be submitting file
meta-data, followed by the actual file, given that the file meta-data has been successfully submitted.  So for each possible file you want to submit you will send:

	* File JSON
	* The actual file

Once you have completed all of these phases successfully, your submission to ENCODE will be complete and the next step would be to have your data wrangler
look over your submission for validation.

Meta-data Objects
=================

Diving deeper into each meta-data object being passed, specific meta-data will be used to create each JSON.  Listing each JSON in order, we include:

	* **Donors**
		* *Information gathered with experiment series*
			* "award":'grant'
			* "lab":'lab'
		* *Information gathered with samples*
			* "organism":'organism'
			* "life_stage":'life_stage'
			* "age":'age'
			* "sex":'sex'

	* **Experiments**
		* *Information gathered with experiment series*
			* "award":'grant'
			* "lab":'lab'
		* *Information gathered with protocols*
			* "assay_term_name":'assay_term_name'
			* "assay_term_id":'assay_term_id'
		* *Information gathered with samples*
			* "biosample_term_name":'biosample_term_name'
			* "biosample_term_id":'biosample_term_id'
			* "biosample_type":'biosample_type'
			* "description":'description'
				
	* **Treatments**
		* *Information gathered with treatments*
			* "treatment_term_name":'treatment_term_name'
			* "treatment_term_id":'treatment_term_id'
			* "treatment_type":'treatment_type'
			* "amount":'concentration'
			* "amount_units":'concentration_units'
			* "duration":'duration'
			* "duration_units":'duration_units'

	* **Biosamples**
		* *Information gathered with experiment series*
			* "award":'grant'
			* "lab":'lab'
		* *Information gathered with protocols*
			* "starting_amount":'starting_amount'
			* "starting_amount_units":'starting_amount_units'
		* *Information gathered with samples*
			* "biosample_term_name":'biosample_term_name'
			* "biosample_term_id":'biosample_term_id'
			* "biosample_type":'biosample_type'
			* "organism":'organism'
			* "derived_from":'biosample_derived_from'
			* "source":'source'
		* *Information gathered with lanes*
			* "date_obtained":'date_received'

	* **Libraries**
		* *Information gathered with experiment series*
			* "award":'grant'
			* "lab":'lab'
		* *Information gathered with samples*
			* "spike-ins":'spike_ins'
			* "size_range":'avg_insert_size'
		* *Information gathered with protocols*
			* "nucleic_acid_term_name":'nucleic_acid_term_name'
			* "nucleic_acid_term_id":'nucleic_acid_term_id'
			* "extraction_method":'extraction_method'
			* "crosslinking_method":'crosslinking_method'
			* "fragmentation_method":'fragmentation_method'

	* **Antibodies**
		* *Information gathered with experiment series*
			* "award":'grant'
			* "lab":'lab'
		* *Information gathered with Antibodies*
			* "source":'source'
			* "product_id":'product_id'
			* "lot_id":'lot_id'
			* "host_organism":'host_organism'
			* "targets":'targets'
			* "clonality":'clonality'
			* "isotype":'isotype'
			* "purifications":'purifications',
			* "url":'url'

	* **Replicates**
		* *Information gathered with samples*
			* "biological_replicate_number":'biological_replica'
			* "technical_replicate_number":'technical_replica'



File Objects
============




Human vs. Non-human Submissions
===============================



The Submission Process
======================



File Submission
===============



Reading the Output
==================


Loading/Viewing the Logs
========================


