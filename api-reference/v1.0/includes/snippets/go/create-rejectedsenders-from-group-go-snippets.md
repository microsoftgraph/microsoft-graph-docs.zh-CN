---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6852b1b1536d1a481ccb108f3757aa5a557f25b
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694869"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/users/alexd@contoso.com",
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).RejectedSenders().$ref().Post(requestBody)


```