---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b66f1acbc9eb61f8782716ef9f909f4dcadba1e2
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226240"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ServicePrincipalRequestBuilderGetQueryParameters{
    Select: "customSecurityAttributes",
}
options := &msgraphsdk.ServicePrincipalRequestBuilderGetOptions{
    Q: requestParameters,
}
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).Get(options)


```