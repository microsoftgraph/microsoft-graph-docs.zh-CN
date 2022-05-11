---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4930c7faff95d114ae99d8a39d1946853ccd7b1f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327987"
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
result, err := graphClient.Education().Schools().Post(requestBody)


```