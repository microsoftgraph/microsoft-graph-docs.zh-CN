---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f000b22f4c881b367b6e2b1e7b04fcfed626b4c2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085434"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewNamedLocation()
displayName := "Updated named location without unknown countries and regions"
requestBody.SetDisplayName(&displayName)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.countryNamedLocation",
    "countriesAndRegions":  []String {
        "CA",
        "IN",
    }
    "includeUnknownCountriesAndRegions": false,
}
options := &msgraphsdk.NamedLocationRequestBuilderPatchOptions{
    Body: requestBody,
}
namedLocationId := "namedLocation-id"
graphClient.Identity().ConditionalAccess().NamedLocationsById(&namedLocationId).Patch(options)


```