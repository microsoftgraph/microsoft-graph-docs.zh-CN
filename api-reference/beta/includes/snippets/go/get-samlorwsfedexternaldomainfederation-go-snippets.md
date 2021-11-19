---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2e812fec528d7ec0f7545dbbdfa72a08b7f0284
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093781"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.IdentityProviderBaseRequestBuilderGetQueryParameters{
    Filter: "domains/any(x:%20x/id%20eq%20'contoso.com')",
}
options := &msgraphsdk.IdentityProviderBaseRequestBuilderGetOptions{
    Q: requestParameters,
}
identityProviderBaseId := "identityProviderBase-id"
result, err := graphClient.Directory().FederationConfigurationsById(&identityProviderBaseId).Get(options)


```