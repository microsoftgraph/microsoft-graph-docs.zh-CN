---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85ea1e93a710abbbd4b74dd52fd4e440f989c87f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082281"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ServicePrincipalsRequestBuilderGetQueryParameters{
    Filter: "startswith(displayName,%20'a')",
    Count: true,
    Top: 1,
    Orderby: "displayName",
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.ServicePrincipalsRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
result, err := graphClient.ServicePrincipals().Get(options)


```