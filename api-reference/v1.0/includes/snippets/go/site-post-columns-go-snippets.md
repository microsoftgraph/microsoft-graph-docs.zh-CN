---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13cd637de13c9cadd95e3ca2cdbe425899af90f8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027130"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewColumnDefinition()
description := "test"
requestBody.SetDescription(&description)
enforceUniqueValues := false
requestBody.SetEnforceUniqueValues(&enforceUniqueValues)
hidden := false
requestBody.SetHidden(&hidden)
indexed := false
requestBody.SetIndexed(&indexed)
name := "Title"
requestBody.SetName(&name)
text := msgraphsdk.NewTextColumn()
requestBody.SetText(text)
allowMultipleLines := false
text.SetAllowMultipleLines(&allowMultipleLines)
appendChangesToExistingText := false
text.SetAppendChangesToExistingText(&appendChangesToExistingText)
linesForEditing := int32(0)
text.SetLinesForEditing(&linesForEditing)
maxLength := int32(255)
text.SetMaxLength(&maxLength)
options := &msgraphsdk.ColumnsRequestBuilderPostOptions{
    Body: requestBody,
}
siteId := "site-id"
result, err := graphClient.SitesById(&siteId).Columns().Post(options)


```