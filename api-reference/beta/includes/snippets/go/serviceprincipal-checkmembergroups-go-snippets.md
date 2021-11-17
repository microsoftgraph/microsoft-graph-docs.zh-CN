---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efff29b4f6a31095df27925010a10e891252f41c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61010833"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetGroupIds( []String {
    "groupIds-value",
}
options := &msgraphsdk.CheckMemberGroupsRequestBuilderPostOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).CheckMemberGroups().Post(options)


```