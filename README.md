# Using graph databases to cross map and Query Disease ontologies
# Load diseases into Neo4j using Prepared_data
Please download Prepared_data.csv
Then Please run Using-graph-databases-to-cross-map-and-Query-Disease-ontologies.py to load dataset in python
# Usage examples
To get disease name, ontology relationships and all other ontology code by code(Progressive supranuclear palsy-pure akinesia with gait freezing syndrome)

    #Example
    if __name__ == "__main__":
        fetch_all_by_known_code("G23.1")
To get ontology relationships and all ontology codes by disease name(Pentalogy of cantrell)

    #Example
    fetch_codes_by_disease_name_with_relations("Pentalogy of cantrell")
To get disease names that exist on multiple ontologies by ontology names("icd-10","umls","ncit")

    #Example
    columns_to_query = ["icd-10","umls","ncit"]
    df = find_diseases_by_columns(columns_to_query)
    df
