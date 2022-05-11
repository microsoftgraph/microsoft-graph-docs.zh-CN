---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e220dcc80f0004174e0ae29fcf3dc0ad27e8918
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326088"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ApplicationsRequestBuilderGetQueryParameters{
    Search: "%22displayName:Web%22",
    Count: true,
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.ApplicationsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
    Headers: headers,
}
result, err := graphClient.Applications().GetWithRequestConfigurationAndResponseHandler(options, nil)


```