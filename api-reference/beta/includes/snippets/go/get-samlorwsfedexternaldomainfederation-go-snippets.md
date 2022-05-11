---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 589e6acba6dc2ef6db7204e4756c65968aa85b61
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325776"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.IdentityProviderBaseRequestBuilderGetQueryParameters{
    Filter: "domains/any(x:%20x/id%20eq%20'contoso.com')",
}
options := &msgraphsdk.IdentityProviderBaseRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
identityProviderBaseId := "identityProviderBase-id"
result, err := graphClient.Directory().FederationConfigurationsById(&identityProviderBaseId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```