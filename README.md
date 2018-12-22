# political-economy_subsidy-reform_ecuador
Estimating the distributional impacts of energy subsidy removal and compensation schemes in Ecuador based on input-output and household data.<br/>

Import files:  
Dictionary Categories.csv, Dictionary ENI-IOT.csv, and Dictionary Subcategories.csv based on [1]  
Dictionary IOT.csv and IOT_2012.csv (cannot be redistruted) based on [2]  
Dictionary Taxes.csv and Dictionary Transfers.csv based on [3]  
ENIGHUR11_GASTOS_V.csv,  ENIGHUR11_HOGARES_AGREGADOS.csv, and ENIGHUR11_PERSONAS_INGRESOS.csv based on [4]  
Price increase scenarios.csv based on [5]<br/>
  
Further basic files and documents:  
[1] 4_M&D_Mapping ENIGHUR expenditures to IOT_180605.xlsm<br/>
[2] Input-output table 2012 (https://contenido.bce.fin.ec/documentos/PublicacionesNotas/Catalogo/CuentasNacionales/Anuales/Dolares/MIP2012Ampliada.xls). Save the sheet with the IOT 2012 (Matriz simétrica) as IOT_2012.csv and edit the format: first column and row: IOT labels<br/>
[3] 4_M&D_ENIGHUR income_180606.xlsx<br/>
[4] ENIGHUR data can be retrieved from http://www.ecuadorencifras.gob.ec/encuesta-nacional-de-ingresos-y-gastos-de-los-hogares-urbanos-y-rurales/  
Household datasets are only available in SPSS file format and the free software PSPP is used to convert .sav- to .csv-files, as this format can be read directly and efficiently into a Python Pandas DataFrame. See PSPP syntax below:  
save translate  
/outfile = filename  
/type = CSV  
	/textoptions decimal = DOT  
	/textoptions delimiter = ';'  
/fieldnames  
/cells=values        
/replace.<br/>
[5] 3_Ecuador_Energy subsidies and 4_M&D_Price scenarios_180610.xlsx  
