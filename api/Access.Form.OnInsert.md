---
title: Form.OnInsert property (Access)
keywords: vbaac10.chm13431
f1_keywords:
- vbaac10.chm13431
ms.prod: access
api_name:
- Access.Form.OnInsert
ms.assetid: 26c0ceb7-f345-2ca8-eb0c-744c60cf5340
ms.date: 03/14/2019
ms.localizationpriority: medium
---


# Form.OnInsert property (Access)

Sets or returns the value of the **Before Insert** box in the Properties window of a form. Read/write **String**.


## Syntax

_expression_.**OnInsert**

_expression_ A variable that represents a **[Form](Access.Form.md)** object.


## Remarks

This property is helpful for programmatically changing the action that Microsoft Access takes when an event is triggered. For example, between event calls you may want to change an expression's parameters, or switch from an event procedure to an expression or macro, depending on the circumstances under which the event was triggered. 

Although the name of this property is **OnInsert**, setting this property actually sets the value of the **Before Insert** box.

The **BeforeInsert** event occurs when the user types the first character in a new record, but before the record is actually created.

The **OnInsert** value will be one of the following, depending on the selection chosen in the Choose Builder window (accessed by choosing the **Build** button next to the **Before Insert** box in the form's Properties window):

- If you choose Expression Builder, the value will be =_expression_, where _expression_ is the expression from the Expression Builder window.
    
- If you choose Macro Builder, the value is the name of the macro. 
    
- If you choose Code Builder, the value will be [Event Procedure]. 
    
If the **Before Insert** box is blank, the property value is an empty string.


## Example

The following example prints the value of the **OnInsert** property in the Immediate window for the **Order Entry** form.

```vb
Debug.Print Forms("Order Entry").OnInsert
```



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]