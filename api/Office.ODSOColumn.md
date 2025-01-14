---
title: ODSOColumn object (Office)
keywords: vbaof11.chm233000
f1_keywords:
- vbaof11.chm233000
ms.prod: office
api_name:
- Office.ODSOColumn
ms.assetid: f8fe41bd-c9bd-fb5b-8ca7-27940c9c0996
ms.date: 01/22/2019
ms.localizationpriority: medium
---


# ODSOColumn object (Office)

Represents a field in a data source. The **ODSOColumn** object is a member of the **ODSOColumns** collection.


## Remarks

The **ODSOColumns** collection includes all the data fields in a mail merge data source (for example, Name, Address, and City).

You cannot add fields to the **ODSOColumns** collection. All data fields in a data source are automatically included in the **ODSOColumns** collection.

Use **[Columns](Office.OfficeDataSourceObject.Columns.md)**(_index_), where _index_ is the data field name or index number, to return a single **ODSOColumn** object. The index number represents the position of the data field in the mail merge data source.


## Example

This example retrieves the name and value of the first field of the first record in the data source attached to the active publication.


```vb
Sub GetDataFromSource() 
 
 Dim appOffice As OfficeDataSourceObject 
 
 Set appOffice = Application.OfficeDataSourceObject 
 appOffice.Open bstrConnect:="DRIVER=SQL Server;SERVER=ServerName;" & _ 
 "UID=user;PWD=;DATABASE=Northwind", bstrTable:="Employees" 
 
 With appOffice.Columns 
 MsgBox "Field Name: " & .Item(1).Name & vbLf & _ 
 "Value: " & .Item(1).Value 
 End With 
End Sub
```


## See also

- [ODSOColumn object members](overview/Library-Reference/odsocolumn-members-office.md)
- [Object Model Reference](overview/Library-Reference/reference-object-library-reference-for-office.md)





[!include[Support and feedback](~/includes/feedback-boilerplate.md)]