---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aca865086384fb0b07eb845692e9da6e098b15ed
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328094"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DeltaRequestBuilderGetQueryParameters{
    Select: "displayName,description,mailNickname",
}
headers := map[string]string{
    "Prefer": "return=minimal"
}
options := &msgraphsdk.DeltaRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
    Headers: headers,
}
result, err := graphClient.Groups().Delta()().GetWithRequestConfigurationAndResponseHandler(options, nil)


```