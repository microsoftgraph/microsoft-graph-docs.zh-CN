---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbdcf9409e0608dd93aea6a31bfe07497a66f756
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326882"
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
result, err := graphClient.Me().Profile().Positions().Post(requestBody)


```