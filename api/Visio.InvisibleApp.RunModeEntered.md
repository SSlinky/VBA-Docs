---
title: InvisibleApp.RunModeEntered event (Visio)
ms.prod: visio
api_name:
- Visio.InvisibleApp.RunModeEntered
ms.assetid: 75bbf305-87c3-9731-ad9a-a55be67323ab
ms.date: 06/08/2017
ms.localizationpriority: medium
---


# InvisibleApp.RunModeEntered event (Visio)

Occurs after a document enters run mode.


## Syntax

_expression_.**RunModeEntered** (_doc_)

_expression_ A variable that represents an **[InvisibleApp](Visio.InvisibleApp.md)** object.


## Parameters



|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _doc_|Required| **[IVDOCUMENT]**|The document that entered run mode.|

## Remarks

If you are using Microsoft Visual Basic or Visual Basic for Applications (VBA), the syntax in this topic describes a common, efficient way to handle events.

If you want to create your own **Event** objects, use the **[Add](visio.eventlist.add.md)** or **[AddAdvise](visio.eventlist.addadvise.md)** method. 

To create an **Event** object that runs an add-on, use the **Add** method as it applies to the **EventList** collection. 

To create an **Event** object that receives notification, use the **AddAdvise** method. 

To find an event code for the event that you want to create, see [Event codes](../visio/Concepts/event-codesvisio.md).

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]