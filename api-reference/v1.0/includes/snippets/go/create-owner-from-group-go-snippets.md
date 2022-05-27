---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c3dac3b0eb89eb8b1d5a3b6a48fe9f211755795
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695036"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}",
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Owners().$ref().Post(requestBody)


```