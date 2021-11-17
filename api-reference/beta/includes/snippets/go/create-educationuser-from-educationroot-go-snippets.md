---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ca9e1bb5b6f364790ae9c92fdac1416f8a9c25d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60986563"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewEducationUser()
displayName := "Dion Matheson"
requestBody.SetDisplayName(&displayName)
givenName := "Dion"
requestBody.SetGivenName(&givenName)
requestBody.SetMiddleName(nil)
surname := "Matheson"
requestBody.SetSurname(&surname)
mail := "DionM@contoso.com"
requestBody.SetMail(&mail)
mobilePhone := "+1 (253) 555-0101"
requestBody.SetMobilePhone(&mobilePhone)
createdBy := msgraphsdk.NewIdentitySet()
requestBody.SetCreatedBy(createdBy)
user := msgraphsdk.NewIdentity()
createdBy.SetUser(user)
displayName := "Susana Rocha"
user.SetDisplayName(&displayName)
id := "14012"
user.SetId(&id)
externalSource := "sis"
requestBody.SetExternalSource(&externalSource)
mailingAddress := msgraphsdk.NewPhysicalAddress()
requestBody.SetMailingAddress(mailingAddress)
city := "Los Angeles"
mailingAddress.SetCity(&city)
countryOrRegion := "United States"
mailingAddress.SetCountryOrRegion(&countryOrRegion)
postalCode := "98055"
mailingAddress.SetPostalCode(&postalCode)
state := "CA"
mailingAddress.SetState(&state)
street := "12345 Main St."
mailingAddress.SetStreet(&street)
primaryRole := "student"
requestBody.SetPrimaryRole(&primaryRole)
residenceAddress := msgraphsdk.NewPhysicalAddress()
requestBody.SetResidenceAddress(residenceAddress)
city := "Los Angeles"
residenceAddress.SetCity(&city)
countryOrRegion := "United States"
residenceAddress.SetCountryOrRegion(&countryOrRegion)
postalCode := "98055"
residenceAddress.SetPostalCode(&postalCode)
state := "CA"
residenceAddress.SetState(&state)
street := "12345 Main St."
residenceAddress.SetStreet(&street)
options := &msgraphsdk.UsersRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Education().Users().Post(options)


```