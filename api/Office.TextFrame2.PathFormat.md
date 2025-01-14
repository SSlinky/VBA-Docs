---
title: TextFrame2.PathFormat property (Office)
ms.prod: office
api_name:
- Office.TextFrame2.PathFormat
ms.assetid: 66148447-5bb8-5e15-0959-e2282fb4bd00
ms.date: 01/25/2019
ms.localizationpriority: medium
---


# TextFrame2.PathFormat property (Office)

Returns or sets the path type for the specified text frame. Read/write.


## Syntax

_expression_.**PathFormat**

_expression_ An expression that returns a **[TextFrame2](Office.TextFrame2.md)** object.


## Remarks

The value of the **PathFormat** property can be one of these **[MsoPathFormat](office.msopathformat.md)** constants. The value **msoPathTypeMixed** cannot be set. Setting the value **msoPathTypeNone** removes any existing path.

- **msoPathType1**    
- **msoPathType2**    
- **msoPathType3**    
- **msoPathType4**    
- **msoPathTypeMixed**    
- **msoPathTypeNone**
    

## See also

- [TextFrame2 object members](overview/Library-Reference/textframe2-members-office.md)



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]