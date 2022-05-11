---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3558e3a47bb369450b28b78aaed1a4b2820da8d9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328779"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MeRequestBuilderGetQueryParameters{
    Expand: "manager($levels=max;$select=id,displayName)",
    Select: "id,displayName",
    Count: true,
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.MeRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
    Headers: headers,
}
result, err := graphClient.Me().GetWithRequestConfigurationAndResponseHandler(options, nil)


```