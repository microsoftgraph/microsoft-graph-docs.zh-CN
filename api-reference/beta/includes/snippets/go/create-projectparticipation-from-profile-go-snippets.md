---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4b3e1695f412e1248877a87ffbc2211f3e1f081
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102281"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewProjectParticipation()
requestBody.SetCategories( []String {
    "Branding",
}
client := msgraphsdk.NewCompanyDetail()
requestBody.SetClient(client)
displayName := "Contoso Ltd."
client.SetDisplayName(&displayName)
department := "Corporate Marketing"
client.SetDepartment(&department)
webUrl := "https://www.contoso.com"
client.SetWebUrl(&webUrl)
displayName := "Contoso Re-branding Project"
requestBody.SetDisplayName(&displayName)
detail := msgraphsdk.NewPositionDetail()
requestBody.SetDetail(detail)
company := msgraphsdk.NewCompanyDetail()
detail.SetCompany(company)
displayName := "Adventureworks Inc."
company.SetDisplayName(&displayName)
department := "Consulting"
company.SetDepartment(&department)
webUrl := "https://adventureworks.com"
company.SetWebUrl(&webUrl)
description := "Rebranding of Contoso Ltd."
detail.SetDescription(&description)
jobTitle := "Lead PM Rebranding"
detail.SetJobTitle(&jobTitle)
role := "project management"
detail.SetRole(&role)
summary := "A 6 month project to help Contoso rebrand after they were divested from a parent organization."
detail.SetSummary(&summary)
options := &msgraphsdk.ProjectsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Projects().Post(options)


```