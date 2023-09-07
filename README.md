# Using graph databases to cross map and Query Disease ontologies
# Load diseases into Neo4j using Prepared_data
Please download Prepared_data.csv
Then Please run Using-graph-databases-to-cross-map-and-Query-Disease-ontologies.py to load dataset in python
# Usage examples
To get disease name and all other ontology code by code
#Example
if __name__ == "__main__":
    fetch_all_by_known_code("G23.1")
