# AirtableMetaMapper
Airtable MetaMapper is a tool that maps and connects the current schema of an Airtable database to metadata tables, facilitating the organization and management of table, view, and field metadata. This is a script meant to be used within the Airtable scripting block.

Airtable MetaMapper is a collection of functions designed to simplify the generation of metadata for tables, views, and fields within an Airtable database. With the help of these functions, users can easily extract and organize essential schema information into a structured metadata format.
Usage
1. Begin by executing the generateBaseschema function. This function retrieves details regarding tables, views, and fields from the Airtable database, creating a metadata object that captures the essential information.
2. Next, execute the createMetadataTables function. This function ensures the existence of metadata tables required to store information about tables, views, and fields. If the tables do not already exist, the function will create them automatically.
3. Utilize the createReferenceDictionary function to generate a dictionary that establishes the connection between specific metadata records and their corresponding IDs. This mapping is crucial for maintaining relationships between different metadata elements.
4. Proceed to execute the populateMetadataTables function. This function populates the metadata tables with the extracted schema information and utilizes the reference dictionary to accurately associate records with their respective tables, views, and fields.
5. Finally, run the generateschemaTable function. This function generates a new record within the metadata schema table, storing the current schema along with a timestamp for future reference and version tracking.
By following these steps, Airtable MetaMapper automates the process of generating and populating metadata tables based on the existing database schema, simplifying the management and organization of essential metadata.
Please note that you may need to make necessary adjustments and customizations to fit your specific use case or requirements.
