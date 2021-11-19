---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e62918fc5f5dee55bc5234ac74a994bd62efc1e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084485"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationalActivity()
institution := msgraphsdk.NewInstitutionData()
requestBody.SetInstitution(institution)
location := msgraphsdk.NewPhysicalAddress()
institution.SetLocation(location)
type := "business"
location.SetType(&type)
location.SetPostOfficeBox(nil)
street := "12000 E Prospect Rd"
location.SetStreet(&street)
city := "Fort Collins"
location.SetCity(&city)
state := "Colorado"
location.SetState(&state)
countryOrRegion := "USA"
location.SetCountryOrRegion(&countryOrRegion)
postalCode := "80525"
location.SetPostalCode(&postalCode)
options := &msgraphsdk.EducationalActivityRequestBuilderPatchOptions{
    Body: requestBody,
}
educationalActivityId := "educationalActivity-id"
graphClient.Me().Profile().EducationalActivitiesById(&educationalActivityId).Patch(options)


```