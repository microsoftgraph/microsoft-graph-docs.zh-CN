---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0a9cfb40aba4cff832ee453a5bc760e5be2b2ad
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083606"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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