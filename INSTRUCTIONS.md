# Build Instructions and Notes

### Operating Principles

To be added. Draw schematic of cooling process and insert here.


Link to [Thermocouple-Datalogger](https://github.com/stafforj/Thermocouple-Datalogger) repository for temperature data aquisition.
Link to [Automated-Relay-Switch](https://github.com/stafforj/Automated-Relay-Switch) repository for blender control.
Link to [PID-blender](https://github.com/DTP587/PID-Blender) repository for blender control.


## Bill of Materials

The BoM is split into the main components for the cooling system and additional components that are optional. These additional parts facilitate coolant recirculation, or if using an external chiller to provide the cooling function. The optional components listed below add greater cost to the build (relative to the main component costs). This cost could be reduced by moving to other types of fittings and tubing (e.g., brass fittings and copper tubing).


### Main items

|Name               |QTY|Description                           |
|:------------------|:-:|:-------------------------------------|
|PETG|1  |PETG filament for 3D printing. 386 grams used to print all components. |
|[Silicon conformal sealant](https://uk.rs-online.com/web/p/conformal-coatings/1247695)|1 |Silicon conformal spray coating. Approximately 100 mL used.|
|[EPDM Pipe Adaptor (1)](https://www.screwfix.com/p/floplast-flexi-adaptor-160mm/1009v)|1  |Flexible EPDM pipe adaptor 160mm.|
|[EPDM Pipe Adaptor (2)](https://www.screwfix.com/p/floplast-underground-flexible-adaptor-120-136mm/19914)|1  |Flexible EPDM pipe adaptor 120-136mm.|
|[Adhesive/Sealant](https://www.screwfix.com/p/soudal-fix-all-high-tack-adhesive-sealant-white-290ml/64585)|1  |High bond strength adhesive/sealant. Approximately 30 mL used.|
|[Thermocouple](https://www.tcdirect.co.uk/product-2-190-1---Mineral-Insulated-Thermocouple-with-Pot-Seal-0-25-0-5-0-75-1-0-1-5-and-3-0mm-diameters)|1  |Type K thermocouple with 3 mm 310 SS probe sheath diameter, 100 mm length.|
|Bag of ice|1  |2 kg bag of ice cubes.|
|Thermocouple reader|1 |Data logger for reading Type K thermocouples. See our [Thermocouple-Datalogger](https://github.com/stafforj/Thermocouple-Datalogger) build for a RPi-based datalogger.
|Kitchen blender |1 |Standard off-the-shelf, [relay-controlled](https://github.com/stafforj/Automated-Relay-Switch), or [PID-controlled](https://github.com/DTP587/PID-Blender).
|Misc.|   | <ul><li>Spanners</li><li>Screwdrivers</li><li>Gloves</li><li>Face mask</li><li>Electrical drill/Rotary tool</li><li>1L water</li></ul>|

### Coolant recirculation (optional)

|Name               |QTY|Description                           |
|:------------------|:-:|:-------------------------------------|
|SS tube|1  |1/4" stainless steel tube. 300mm length used. |
|[SS Bulkhead Union](https://buy.ham-let.com/774lss1-4)|2  |Bulk head fittings mounted to top 3DP part.|
|[SS Tube stub adapter](https://buy.ham-let.com/130ltss1-4x1-4)|2  |1/4" Hose barb fitting.|
|[SS Union Tee](https://buy.ham-let.com/764lss1-4)|2  |1/4" Tee fitting.|
|[SS Reducer](https://buy.ham-let.com/767ltss1-16x1-4tc)|2  |1/16" to 1/4" tube fitting.|
|[Thermocouple](https://uk.rs-online.com/web/p/thermocouples/3971501)|2  |Type K thermocouple with 1.5mm SS probe sheath diameter, 150mm length.|
|Tubing|1  |Silicon or Tygon tubing or similiar. 3m length used, 6mm or 1/4" ID. |
|Pump|1  |Pump of choice to recirculate coolant. |
|Misc.|   | <ul><li>Spanners</li><li>Screwdrivers</li></ul>|

## Design & Construction

### CAD files

A total of six components from the cooling system are 3D printed parts. The CAD (.stl) files for printing these parts are located within the folder `./CAD/`.

### Construction

The CAD files were printed using a fused-deposition-modeling (FDM) printer (Ultimaker S3, 0.2mm layer thickness, 20\% infill, no supports). Polyethylene terephthalate glycol (PETG) was selected as the filament material for the printing process due to its ability to tolerate high temperatures (~ 70-80 °C), its mechanical properties, and chemical resistance to certain oils and solvents. 

In this build, the components are exposed to water and ice. Although PETG is compatible with water, the layers resulting from the FDM process can create sites for fluid leakages in the finished part. To remove the risk of leaks, the 3D printed parts were coated with a thin film silicon-based conformal coating (three spray coats ~ 100 microns thickness). To show the visual effect of this, a sample part was 3D printed, masked, and partially covered with a single spray coat (~ 25 microns). The difference between the coated and uncoated PETG surface is shown in the image below. The conformal coating covers the layers and insterstices, sealing the printed part and preventing liquid leaks. This surface coating is mechanically robust. As the surfaces in contact with the coolant and product are a different material than PETG, the chemical resistance of coated parts should be re-assessed for applications where a coolant other than water/ice is used.    

![Conformal coating](./Images/FDM-conformal-coating.png)

Once printed, the parts were coated with three spray coats and allowed to cure at room temperature for 24 hours between coatings. All components of the cooling system are shown in the image below.

![Component breakdown](./Images/all-vessel-components.png)

Components `1`, `4` and `9` were bonded to the synthesis vessel (Kenwood BLP31.D0WG) using a sealant adhesive. The vessel spout with integrated thermocouple mounting (Component `4`), required modifications to the synthesis vessel before the bonding process. A 15 mm diameter hole was drilled at the top and centre of the vessel. This hole allows filling the vessel with precursor materials from the top (shown later). A second 4 mm diameter hole, located 20 mm (centre-to-centre) from the centre of the vessel, was drilled to accomodate the thermocouple probe insertion for measuring process temperature.  The thermocouple probe is inserted into component `4` at the desired depth, and the part then bonded to the top of the vessel. 

![Bonding construction](./Images/FDM-vessel-bonding.png)

The complete assembly instructions are discussed in the following sections. The following image shows the barebone assembly of printed parts and synthesis vessel without EPDM pipe adapters. The design of the spout also facilitates product sampling during processing using a 10 mL pipette.   

![Barebones without EPDM cylinders](./Images/barebones-with-pipette.png)

## Assembly of Liquid Phase Exfoliation Cooling System 

(1) - base 
(2) - mid-section
(3) - top
(4) - vessel spout
(5) - TC insert
(6) - TC plug
(7) - lower cylinder
(8) - upper cylinder

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




