---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b856a01d252232c21f4ae2924984904042fc1053
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315142"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DeltaRequestBuilderGetQueryParameters{
    Select: "displayName,jobTitle,mobilePhone",
}
headers := map[string]string{
    "Prefer": "return=minimal"
}
options := &msgraphsdk.DeltaRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
    Headers: headers,
}
result, err := graphClient.Users().Delta()().GetWithRequestConfigurationAndResponseHandler(options, nil)


```