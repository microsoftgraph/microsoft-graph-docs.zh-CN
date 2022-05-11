---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea649feac9a7e10e0dc60dad2909ada3e1d50cb8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328124"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.EventsRequestBuilderGetQueryParameters{
    Select: "subject,body,bodyPreview",
}
headers := map[string]string{
    "Prefer": "outlook.body-content-type="text""
}
options := &msgraphsdk.EventsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
    Headers: headers,
}
result, err := graphClient.Me().Events().GetWithRequestConfigurationAndResponseHandler(options, nil)


```