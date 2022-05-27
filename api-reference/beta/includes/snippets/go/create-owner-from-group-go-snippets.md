---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e974ab1ac78e406447d7e3d9aac34c30ac08a4d3
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695092"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/users/{id}",
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Owners().$ref().Post(requestBody)


```