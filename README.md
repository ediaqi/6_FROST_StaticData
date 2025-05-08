# 6_FROST_StaticData
Script that creates the json payload for the creation of static STA entities via API.

### Generation of static JSONsons for entity creation on FROST  
The scripts generate static JSON files, which can be used with **POSTMAN**, for the creation of basic entities on **FROST** for the various pilots of the project.

#### Basic Entities to be Created (One-Time):  
- **Things**  
- **Locations**  
- **Feature of Interest (FOI)**  
- **Observed Properties**  
- **Datastreams**  

#### Execution Procedure
The scripts are based on **Excel files**, so before executing them, it is necessary to:  
1. **Start a Jupyter Notebook instance.**  
2. **Run each cell of the script:** follow the order of the cells as defined in the notebook, ensuring that no errors occur during execution.
3. **Specify the correct paths to the Excel files** that were initially filled in by each pilot in the cells. 

#### Differences Between the Pilots 
- **Seville**: the geometry of the locations is represented by a **MultiLineString**.  
- **Vilnius**: the geometry can be either a **Point** or a **Polygon**, depending on the case.  

#### Customizations and Modifications
- It is possible to modify the output file names.
- It might be necessary to update the unique IDs, for example changing "THI.FE.001" to "THI.ZG.001".  
- It is important to update the counters to maintain data consistency.
- It is important to modify the sensor indication when creating the Datastreams.

