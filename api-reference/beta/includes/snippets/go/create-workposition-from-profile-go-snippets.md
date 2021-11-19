---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c64869735cce080ddcdbc70c11c1225c08ff91ec
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091605"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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