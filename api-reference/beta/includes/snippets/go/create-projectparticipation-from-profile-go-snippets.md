---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b56b0f5b55ff64c96f50d0b6d1de3c2ce5be1699
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60996980"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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