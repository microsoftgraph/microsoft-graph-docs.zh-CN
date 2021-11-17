---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a61a6bcfd42a752d69c88f9982248f34fa0637e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024274"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.ServicePrincipalsRequestBuilderGetQueryParameters{
    Search: "%22displayName:Team%22",
    Count: true,
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