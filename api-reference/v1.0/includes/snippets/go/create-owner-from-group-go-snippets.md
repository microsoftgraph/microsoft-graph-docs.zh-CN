---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 102fa0d118037bfc31accba9ea1b18be54b20484
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082886"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}",
}
options := &msgraphsdk.RefRequestBuilderPostOptions{
    Body: requestBody,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Owners().$ref().Post(options)


```