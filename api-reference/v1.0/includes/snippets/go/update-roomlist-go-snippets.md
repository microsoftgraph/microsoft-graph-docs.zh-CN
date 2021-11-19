---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 841e69ba770e847d1f73654793a5fa9c3915c878
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091199"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPlace()
displayName := "Building 1"
requestBody.SetDisplayName(&displayName)
phone := "555-555-0100"
requestBody.SetPhone(&phone)
address := msgraphsdk.NewPhysicalAddress()
requestBody.SetAddress(address)
street := "4567 Main Street"
address.SetStreet(&street)
city := "Buffalo"
address.SetCity(&city)
state := "NY"
address.SetState(&state)
postalCode := "98052"
address.SetPostalCode(&postalCode)
countryOrRegion := "USA"
address.SetCountryOrRegion(&countryOrRegion)
geoCoordinates := msgraphsdk.NewOutlookGeoCoordinates()
requestBody.SetGeoCoordinates(geoCoordinates)
geoCoordinates.SetAltitude(nil)
latitude := float64(47)
geoCoordinates.SetLatitude(&latitude)
longitude := float64(-122)
geoCoordinates.SetLongitude(&longitude)
geoCoordinates.SetAccuracy(nil)
geoCoordinates.SetAltitudeAccuracy(nil)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.roomList",
}
options := &msgraphsdk.PlaceRequestBuilderPatchOptions{
    Body: requestBody,
}
placeId := "place-id"
graphClient.PlacesById(&placeId).Patch(options)


```