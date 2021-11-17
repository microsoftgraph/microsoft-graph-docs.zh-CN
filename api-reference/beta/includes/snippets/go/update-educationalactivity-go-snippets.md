---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 313f0daf95daf94e50b3491a6d50a2092fe13619
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61005213"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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