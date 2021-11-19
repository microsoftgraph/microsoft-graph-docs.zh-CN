---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a9c3707d907b0e20c401e85936d7a72b79b6eaa
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100999"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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