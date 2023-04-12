For the webElements functions to work correctly, you need to enable "Passthrough HTML" on your SAP BI / BOBJ Enteprise system. This is what enables HTML in single line formulas & fields to be interpreted as such. WebElements is a Custom Function library that utilizes the Passthrough HTML feature.

These steps should be done by your SAP BI Administrator.

1. Create a new text file named CrystalReports.properties in the following directory.
```
<install directory>\SAP BusinessObjects Enterprise XI 4.0\warfiles\webapps\BOE\WEB-INF\config\custom
```
  
2. The content of this file should be as follows

```
# This parameter is used to activate pass-through HTML for Crystal Reports
  
crystal_encode_html_for_single_line_field_objects=no
```
  
3. Run wdeploy.
