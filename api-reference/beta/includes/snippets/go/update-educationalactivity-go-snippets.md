---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 845a0bfce7daff81a892d4e684897e98dd23c54b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411664"
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
result, err := graphClient.Me().Profile().EducationalActivitiesById(&educationalActivityId).Patch(options)


```