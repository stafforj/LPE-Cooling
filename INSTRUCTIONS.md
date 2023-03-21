# Build Instructions and Notes

### Operating Principles

To be added. 

Draw schematic of cooling process and insert here.

Link to [Thermocouple-Datalogger](https://github.com/stafforj/Thermocouple-Datalogger) repository for temperature data aquisition.
Link to [Automated-Relay-Switch](https://github.com/stafforj/Automated-Relay-Switch) repository for blender control.
Link to [PID-blender](https://github.com/DTP587/PID-Blender) repository for blender control.


## Bill of Materials

The BoM is split into the main components of the build and additional components that are optional. These additional parts facilitate coolant recirculation, or if using an external chiller to provide the cooling function. The optional components listed below add a notable cost to the build (relative to the main component costs). This cost could be reduced by moving to other fittings and tubing (e.g., brass fittings and copper tubing).

### Main items

|Name               |QTY|Description                           |
|:------------------|:-:|:-------------------------------------|
|[PETG](RS components link)|1  |PETG filament for 3D printing. 386 grams used for all components. |
|[Silicon conformal sealant](MG chemicals)|1 |Silicon conformal spray coating.|
|[EPDM Pipe Adaptor (1)](Screwfix)|1  |Flexible EPDM pipe adaptor 160mm.|
|[EPDM Pipe Adaptor (2)](Screwfix)|1  |Flexible EPDM pipe adaptor 120-136mm.|
|[Adhesive/Sealant](Screwfix)|1  | High bond strength adhesive/sealant.|
|[Thermocouple](TC direct)|1  |Type K thermocouple with 3mm SS probe sheath diameter.|
|Bag of ice|1  |2 kg bag of ice cubes.|
|[Thermocouple reader](Link to Thermcouple Datalogger build)|1 | Data logger for reading Type K thermocouples.
|Misc.|   | <ul><li>Spanners</li><li>Screwdrivers</li></ul>|

### Coolant recirculation (optional)

|Name               |QTY|Description                           |
|:------------------|:-:|:-------------------------------------|
|[SS tube](RS components link)|1  |1/4" stainless steel tube. 300mm length used. |
|[SS fitting](Hamlet)|2  |Bulk head fittings mounted to top 3DP part.|
|[SS fitting](Hamlet)|2  |1/4" Hose barb fitting.|
|[SS fitting](Hamlet)|2  |1/4" Tee fitting.|
|[SS fitting](Hamlet)|2  |1/16" to 1/4" tube fitting.|
|[Thermocouple](RS components)|2  |Type K thermocouples with 1.5mm SS probe sheath diameter.|
|Tubing|1  |Silicon or Tygon tubing or similiar. 3m length used, 6mm or 1/4" ID. |
|Pump|1  |Pump of choice to recirculate coolant. |
|Misc.|   | <ul><li>Spanners</li><li>Screwdrivers</li></ul>|

## Design & Construction

### CAD files

A total of six components from the cooling system are 3D printed parts. The CAD (.stl) files for printing these parts are located within the folder `./CAD/`.

### Construction

86g (base) + 42g (spout) + 181g (middle) + 8g (x2 ports) + 69g (top) = 386 g

To be added. Figure comparing conformally coated FDM to standard PETG.

The CAD files were printed using a Fused-deposition-modeling (FDM) printer (Ultimaker S3, 0.2mm layer thickness, 20\% infill, no supports). PETG was selected as the filament material for the printing process due to its ability to tolerate high temperatures (~ 70-80 °C), mechanical properties, and good chemical resistance to certain oils and solvents. 

In this build, the components are exposed to water and ice. Although PETG is compatible with this, the layers in the FDM process can create sites for fluid leakages. To remove the risk of leakages, the 3D printed parts were coated with a silicon conformal coating. 



![Conformal coating](./Images/FDM-conformal-coating.png)

![Bonding construction](./Images/FDM-vessel-bonding.png)

![Barebones without EPDM cylinders](./Images/barebones-with-pipette.png)

![Component breakdown](./Images/all-vessel-components.png)

## Assembly of Liquid Phase Exfoliation Cooling System 

### Steps 1-4: Cooling jacket assembly

To be added.

![Assembling jacket](./Images/pre-test-assembly.png)

### Step 5: Precursor filling

To be added.

![Fill internal vessel](./Images/pre-test-assembly-precursor-fill.png)

### Step 6: Ice filling

To be added.

![Ice packing](./Images/pre-test-assembly-ice.png)

### Step 7: Cooling jacket closure

To be added. Connection of pump tubes for coolant circulation.

![Top insertion](./Images/pre-test-assembly-close-vessel.png)

### Step 8-9: Thermocouple routing 

To be added.

![TC plugging](./Images/pre-test-assembly-route-TC.png)

### Step 10: Connecting to thermocouple datalogger

To be added.

![TC connections](./Images/pre-test-assembly-tc-connections.png)




