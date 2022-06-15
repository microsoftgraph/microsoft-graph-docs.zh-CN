---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e6407d248e60a60b208f1f96e1c0d053d434714
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098797"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewList()
displayName := "Books"
requestBody.SetDisplayName(&displayName)
requestBody.SetColumns( []ColumnDefinition {
    msgraphsdk.NewColumnDefinition(),
name := "Author"
    SetName(&name)
text := msgraphsdk.NewTextColumn()
    SetText(text)
    msgraphsdk.NewColumnDefinition(),
name := "PageCount"
    SetName(&name)
number := msgraphsdk.NewNumberColumn()
    SetNumber(number)
}
list := msgraphsdk.NewListInfo()
requestBody.SetList(list)
template := "genericList"
list.SetTemplate(&template)
siteId := "site-id"
result, err := graphClient.SitesById(&siteId).Lists().Post(requestBody)


```