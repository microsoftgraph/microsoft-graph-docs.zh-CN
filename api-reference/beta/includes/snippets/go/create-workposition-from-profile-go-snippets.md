---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb668040c534ee1a379e4a84556a8cc1d73d9f9a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027907"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewWorkPosition()
detail := msgraphsdk.NewPositionDetail()
requestBody.SetDetail(detail)
company := msgraphsdk.NewCompanyDetail()
detail.SetCompany(company)
displayName := "Adventureworks Ltd."
company.SetDisplayName(&displayName)
department := "Consulting"
company.SetDepartment(&department)
officeLocation := "AW23/344"
company.SetOfficeLocation(&officeLocation)
address := msgraphsdk.NewPhysicalAddress()
company.SetAddress(address)
type := "business"
address.SetType(&type)
street := "123 Patriachy Ponds"
address.SetStreet(&street)
city := "Moscow"
address.SetCity(&city)
countryOrRegion := "Russian Federation"
address.SetCountryOrRegion(&countryOrRegion)
postalCode := "RU-34621"
address.SetPostalCode(&postalCode)
webUrl := "https://www.adventureworks.com"
company.SetWebUrl(&webUrl)
jobTitle := "Senior Product Branding Manager II"
detail.SetJobTitle(&jobTitle)
role := "consulting"
detail.SetRole(&role)
isCurrent := true
requestBody.SetIsCurrent(&isCurrent)
options := &msgraphsdk.PositionsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Positions().Post(options)


```