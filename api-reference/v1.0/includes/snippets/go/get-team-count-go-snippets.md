---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 447f7aecf3adc8b3f6394c41afc31474671af3e4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085518"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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