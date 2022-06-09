# Get the data


## Structure

* :page_with_curl: **`df_clinical.tsv`**: clinical dataframe in tab seperated text format.

Each row is a patient and each column a descriptor.

Details about descriptor are as follows:

	* ID the unique ID of each patient/sample
	* SEX, AGE demographics
	* Mds type
	* WHO 2016 classification
	* Blood counts and Blast counts
	* Cytogenetics
	* IPSS-R risk category and score
	* IPSS-M risk category and score
	* NGS derived deletions, gains and regions copy-neutral loss of heterozygosity as a list of chr. arms (CNACS)
	* Annotation of complex karyotype
	* Status of chr.17 at the TP53 locus
	* Treatment status regarding HMA, Lenalidomid, Chemo, HSCT
	* Overall survival, Leukemia free surival, and AML transformation information


* :clipboard: **`df_mut.tsv`**: binary matrix of mutated genes. Patients in lines and genes in columns. The file is tab seperated.


* :clipboard: **`df_cna.tsv`**: binary matrix of cytogenetics alterations. Patients in lines and alterations in columns. The file is tab seperated.


* :bar_chart: **`maf.tsv`**: mutation file.

Each row corresponds to a given mutation in a given patient.

Details about mutation fields  are as follows:

	* ID the unique ID of each patient/sample
	* CHR START END REF ALT the genomic position and descriptor of the mutation
	* GENE 
	* cDNA_CHANGE
	* PROTEIN_CHANGE 
	* VT variant type (substitution, indels)
	* EFFECT classification of mutation consequence, ie missense nonsense frameshift ...
	* VAF DEPTH variant allele frequency and coverage depth
