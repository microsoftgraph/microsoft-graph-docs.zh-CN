---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da621e45cd4815b59ae816673d214a8171e6d184
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694440"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/users/alexd@contoso.com",
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).AcceptedSenders().$ref().Post(requestBody)


```