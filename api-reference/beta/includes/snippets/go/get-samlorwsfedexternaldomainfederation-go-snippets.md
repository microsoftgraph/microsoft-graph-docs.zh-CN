---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d9294536d757452d9a85e4017e1199b9f09ccd9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032087"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.IdentityProviderBaseRequestBuilderGetQueryParameters{
    Filter: "domains/any(x:%20x/id%20eq%20'contoso.com')",
}
options := &msgraphsdk.IdentityProviderBaseRequestBuilderGetOptions{
    Q: requestParameters,
}
identityProviderBaseId := "identityProviderBase-id"
result, err := graphClient.Directory().FederationConfigurationsById(&identityProviderBaseId).Get(options)


```