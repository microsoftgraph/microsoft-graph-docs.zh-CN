---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52b246b52e5892b7b61ccf946a0e8b17fca0ace6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120720"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationSchool()
displayName := "Fabrikam High School"
requestBody.SetDisplayName(&displayName)
description := "Magnate school for the arts. Los Angeles School District"
requestBody.SetDescription(&description)
externalSource := "String"
requestBody.SetExternalSource(&externalSource)
principalEmail := "AmyR@fabrikam.com"
requestBody.SetPrincipalEmail(&principalEmail)
principalName := "Amy Roebuck"
requestBody.SetPrincipalName(&principalName)
externalPrincipalId := "14007"
requestBody.SetExternalPrincipalId(&externalPrincipalId)
highestGrade := "12"
requestBody.SetHighestGrade(&highestGrade)
lowestGrade := "9"
requestBody.SetLowestGrade(&lowestGrade)
schoolNumber := "10002"
requestBody.SetSchoolNumber(&schoolNumber)
address := msgraphsdk.NewPhysicalAddress()
requestBody.SetAddress(address)
city := "Los Angeles"
address.SetCity(&city)
countryOrRegion := "United States"
address.SetCountryOrRegion(&countryOrRegion)
postalCode := "98055"
address.SetPostalCode(&postalCode)
state := "CA"
address.SetState(&state)
street := "12345 Main St."
address.SetStreet(&street)
externalId := "10002"
requestBody.SetExternalId(&externalId)
phone := "+1 (253) 555-0102"
requestBody.SetPhone(&phone)
options := &msgraphsdk.SchoolsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Education().Schools().Post(options)


```