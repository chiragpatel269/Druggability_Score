1. #Number of unique drugs with their status and having at least 1 target, transporter or enzyme associated
   drugs.csv --> 7485 such drugs with metadata information (id,drugname,drug_type,approved,experimental,illicit,investigational,nutraceutical,withdrawn)

2. #Proteins interacting with drugs either as target, enzyme or transporter
   partner_protein.csv --> 4,632 such targets with metadata information (partner_id,partner_name,gene_name,uniprot_id,genbank_gene_id,genbank_protein_id,hgnc_id,organism,taxonomy_id)

3. #Protein interacting with drugs either as target, enzyme or transporter and organism associated is Human
   partner_protein_human.csv --> 3,033 such targets with metadata information (partner_id,partner_name,gene_name,uniprot_id,genbank_gene_id,genbank_protein_id,hgnc_id,organism,taxonomy_id)

4. #MoA of all drugs
   drug_MOA_Description.csv --> 24,855 such entires with metadata (id | name | description | indication | pharmacodynamics | mechanism_of_action | protein_binding | toxicity). All the metadata is in text format and makes a good resource for cross-modal RAG models i.e. image or SMILES of drug along with toxicity/moa as text as input and finding MOA or toxicity of analog of the drug

5. #Drug-target information
   drug2target.csv --> 18,137 drug-target interactions independent of species with metadata information (id,partner_id,gene_name,inhibitor,antagonist,agonist)

6. #Drug-target information for humans
   drug2target_human.csv --> 14,576 drug-target interactions with human targets along with metadata information (id,partner_id,gene_name,inhibitor,antagonist,agonist)

7. #Drug-enzyme information
   drug2enzyme.csv --> 4,929 drug-enzyme interactions independent of species along with metadata information (id,partner_id,gene_name,inhibitor,antagonist,agonist)

8. #Drug-enyzme information for humans
   drug2enzyme_human.csv --> 4,870 drug-enyzme interactions with human enxymes along with metadata information (id,partner_id,gene_name,inhibitor,antagonist,agonist)

9. #Drug-transported information
   drug2transporter.csv --> 2,745 drug-transporter interactions independent of species along with metadata information (id,partner_id,gene_name,inhibitor,antagonist,agonist)

10.#Drug-transported information
   drug2transporter_human.csv --> 2,728 drug-transporter interactions independent of species along with metadata information (id,partner_id,gene_name,inhibitor,antagonist,agonist)

11.#Drug smiles information
   smiles.csv --> Drugs with SMILES representations along with metadata information about calculated properties (id|name|cas|smiles|logP ALOGPS|logP ChemAxon|solubility ALOGPS|pKa (strongest acidic)|pKa (strongest basic))

12.StringDB interactions
   StringDB_interactions.csv --> Protein - Protein interaction network  obtained from String PPI with confidence score >=400

13. StringDB proteins
   StringDB_protein_info.csv --> Protein along with metadata information for all proteins available via StringDB and present in the interaction network (#string_protein_id | preferred_name | protein_size )

14. Alphafold uniprot ids
   AlphaFold_UniProtIDs.csv --> Uniprot ids of proteins with structure predicted by AlphaFold2.

15.AlphaFold UnitProtKB
   Curated_AlphaFold_UniProtKB.csv -->  Uniprot id, gene name, details ...

16. subset StringDB interactions
   subset_StringDB_interactions.csv --> Protein -  Protein interaction network of genes which have a mapped UniProtId in AlphaFold Database

17. subset String proteins
   subset_String_protein_info.csv --> Protein along with metadata information for all proteins available via StringDB and mapped to UniProtId in Alphafold Database and present in the interaction network (#string_protein_id | preferred_name | protein_size)

18. Filtered Alphafold Database
   Filtered_AlphaFold_UniProtKB.csv --> Uniprot Ids of proteins in AlphaFold Database matching with at least one gene in StringDB.

19. StringDB genes AlphaFold Mapping
   StringDB_genes_AlphaFold_mapping.csv --> StringDB genes and their mapping to AlphaFold Database Uniprot Ids.
