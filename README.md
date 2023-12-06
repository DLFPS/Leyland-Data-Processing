# Leyland-Data-Processing

## Data Download
1. Login to https://cbm.checkit.net/weblogin
2. Select ESTATE: Waitrose, GROUP: All Buildings, BUILDING: 0775 - WR Leyland RDC, then press electricity meters
3. Select Date Range, from first of the month to end of the month
4. Select Half Hourly Date (By default)
5. Select the following three meters and download one by one (the button next to question mark)
- DB 1-12 Sitewide Trailer Hookup Points_DB 1-12 Sitewide Trailer Hookup Points
- Trailer Hook Up Points BusBar East_Trailer Hook Up Points BusBar East
- Trailer Hook Up Points BusBar West_Trailer Hook Up Points BusBar West

## Data Processing
1. Move the downloaded file to a new folder that the notebook loacted, note that the new folder should only contains the three new downloaded files
2. Change the code ```folder_path = 'New Folder Name'``` in second cell to the new folder name.
3. Change the code ```target_month = 11``` and ```target_year = 2023``` in the last cell to the currerent month.
4. Create a folder named 'output' (could be modified if want to by the last line of code)
5. Run the entire notebook
6. Check that the file 't_checkit_meter_consumption_detail_yyyy_mm.csv' have been created in the output folder

## Data Uploading
1. Login to the datalake with the following location: datalakeblob / JLP / Projects / Leyland
2. Upload the file 't_checkit_meter_consumption_detail_yyyy_mm.csv' to the matched year and month folder
3. Complete! 
