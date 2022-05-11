---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e09bae6a38f8de2128bfd6d1c962cb12fea72f1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326563"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.RiskyUsersRequestBuilderGetQueryParameters{
    Filter: "riskLevel%20eq%20microsoft.graph.riskLevel'medium'",
}
options := &msgraphsdk.RiskyUsersRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.IdentityProtection().RiskyUsers().GetWithRequestConfigurationAndResponseHandler(options, nil)


```