## House Numbering System Workflow

Follow the steps below to implement the house numbering system:

1. **Required Data**
   Ensure you have two datasets:

   * Road network data
   * Building centroid data (or gate location points)

2. **Geometry Validation**
   Clean and fix geometries in the road dataset. Invalid geometries may cause errors during Python processing.

3. **Data Preparation**

   * Add a column named **`Unique_ID`** to the road dataset.
   * Assign a unique identifier to each road segment.
   * Ensure the column name is exactly **`Unique_ID`** (case-sensitive).
   * Include road classification data (`A`, `B`, `C`, `D`) in a column named **`road_class`** (also case-sensitive).

4. **Source Code**
   Open the script:
   **`Complete_Final for 3 Road_Centroid_Ward14`**

5. **Install Dependencies**
   Install all required Python libraries before running the script.

6. **Update Input Paths**
   In **Step 1** of the script, update the file paths to match the location of your input datasets.

7. **Update Output Paths**
   In **Steps 9 and 10**, specify the desired output directories where results will be saved.

8. **Run the Script**
   Execute the script. Output shapefiles (`.shp`) will be generated and saved locally.

9. **Load Output in GIS**
   Import the generated shapefiles into your GIS software.

10. **Output Details**
    The script produces:

* Point data containing assigned house numbers
* Line data linking buildings to their corresponding roads

The point dataset also includes the **third-level hierarchy road `Unique_ID`, which can be used to join with the original road dataset to retrieve road names.
