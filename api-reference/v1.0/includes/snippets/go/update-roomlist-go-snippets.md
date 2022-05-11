---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb9f842138482bc32fed20a9a6843fc744b1967c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328664"
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
placeId := "place-id"
graphClient.PlacesById(&placeId).Patch(requestBody)


```