---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02fdc51d4c70becad9a6ca8e70a13c579a3a39a9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026774"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewNamedLocation()
displayName := "Named location with unknown countries and regions"
requestBody.SetDisplayName(&displayName)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.countryNamedLocation",
    "countriesAndRegions":  []String {
        "US",
        "GB",
    }
    "includeUnknownCountriesAndRegions": true,
}
options := &msgraphsdk.NamedLocationsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Identity().ConditionalAccess().NamedLocations().Post(options)


```