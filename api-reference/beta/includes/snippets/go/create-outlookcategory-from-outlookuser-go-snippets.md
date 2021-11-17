---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0647175dd9174f2b3d10feb33f24ce394845678e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033983"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewOutlookCategory()
displayName := "Project expenses"
requestBody.SetDisplayName(&displayName)
color := "preset9"
requestBody.SetColor(&color)
options := &msgraphsdk.MasterCategoriesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Outlook().MasterCategories().Post(options)


```