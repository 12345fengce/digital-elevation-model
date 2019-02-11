# Digital Elevation Model Tools

This is the **Python** implementation of **Digital Elevation Model (DEM)** tools.

### Important Terms and Abbrevations:

| Term                                   | Abbrevation | Remark 
| -------------------------------------- | :---------: | :----: 
| Digital Elevation Model                | DEM         | 
| Geographic Coordinate System           | GCS         | [Longitude, Latitude, Elevation] on 3D spheriod
| Projected Coordinate System            | PCS         | [X-axis, Y-axis, Elevation] on 2D plane
| Georeferenced Tagged Image File Format | GeoTIFF     | DEM data format
| World Geodetic System 1984             | WGS-84      | GCS, approximating the spheriod of earth
| Web Mercator or Pseudo Mercator        |             | PCS of WGS-84
| Ordnance Survey Great Britain 1936     | OSGB-36     | GCS, approximating the spheriod of UK
| British National Grid                  | BNG         | PCS of OSGB-36

### Functions:

1. **Transforming** DEM from current GCS (e.g., WGS-84) to another GCS (e.g., OSGB-36).

2. **Projecting** DEM from current GCS (e.g., OSGB-36) to the corresponding PCS (e.g., BNG).

3. **Visuzlising** DEM in PCS as 2D image.

4. **Reading** elevation of specific locations from DEM in GCS.

## DEM Dataset - ASTER GDEM

The Advanced Spaceborne Thermal Emission and Reflection Radiometer (ASTER) Global Digital Elevation Model (GDEM), i.e., ASTER GDEM or ASTGDEM, is a product of the Ministry of Economy, Trade, and Industry (METI) in Japan and the National Aeronautic and Space Administration (NASA) in United States. It is collected by the **Advanced Spaceborne Thermal Emission and Reflection Radiometer** on the NASA spacecraft **Terra**. ASTGDEMv1 was released on 2009 and ASTGDEMv2 was released on 2011.

The ASTER GDEM covers land surfaces between **83°N** and **83°S**. It is comrised of 22702 **1°x1° tiles**. Each tile contains at least 0.01% land surface. Do not be surprised that tiles which contain only ocean area are missing. 

The data format of ASTER GDEM is **GeoTIFF (.tif)**.
