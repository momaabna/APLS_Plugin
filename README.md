# Average Path Length Similarity (APLS) Plugin for QGIS Software


QGIS Plugin for Extracted roads evaluation using APLS matrix 

## Requrements 
- QGIS 3.0 or higher

## Usage
- Before openning the plugin make sure Python console is opened
- Run the plugin and specify inputs correctly  
        ex:Ground truth: /main_folder/Predicted_shp/
            Predicted : /main_folder/test_shp/
            Djkstra Tolerance : 0.0
            Snapping Tolerance : 8.0
- Run and wait untill processing is finished
- The results are displayed in Python console
Results example :
```sh

Processing total of : 49 images.
Apls for Folder : 18178780_15  is  0.9886363636363636
Apls for Folder : 11278840_15  is  0.11675731021559
Apls for Folder : 23278915_15  is  0.3240173376386126
Apls for Folder : 18478900_15  is  0.9666666666666667
................
Apls for Folder : 24628885_15  is  0.07408254856578367
Apls for Folder : 22228900_15  is  0.4204545454545454
Apls for Folder : 24479215_15  is  0.1971564400253033
AVG APLS is 0.4584244128431006
```

## Inputs 

- Ground truth folder contains sub-folders each sub-folder contain shapefile
- Predicted network folder which contains sub-folders each sub-folder contain shapefile
- Djkstra Algorithm Tolerance
- Snapping Tolerance

Example of Folder Structure for the files 
```sh
/main_folder
│   └── test_shp/
│       ├── 10378780_15
│       │   ├── 10378780_15.cpg
│       │   ├── 10378780_15.dbf
│       │   ├── 10378780_15.prj
│       │   ├── 10378780_15.shp
│       │   ├── 10378780_15.shx
│       ├── 10828720_15
│       │   ├── 10828720_15.cpg
│       │   ├── 10828720_15.dbf
│       │   ├── 10828720_15.prj
│       │   ├── 10828720_15.shp
│       │   ├── 10828720_15.shx
-----------------------------------
│   └── Predicted_shp/
│       ├── 10378780_15
│       │   ├── 10378780_15.cpg
│       │   ├── 10378780_15.dbf
│       │   ├── 10378780_15.prj
│       │   ├── 10378780_15.shp
│       │   ├── 10378780_15.shx
│       ├── 10828720_15
│       │   ├── 10828720_15.cpg
│       │   ├── 10828720_15.dbf
│       │   ├── 10828720_15.prj
│       │   ├── 10828720_15.shp
│       │   ├── 10828720_15.shx

```
Screenshot

![alt text](https://github.com/momaabna/APLS_Plugin/raw/main/images/apls.png)