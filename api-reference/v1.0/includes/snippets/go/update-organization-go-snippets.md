---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 976f27acd63e5077913d72105adab118557b1dc8
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412727"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOrganization()
requestBody.SetMarketingNotificationEmails( []String {
    "marketing@contoso.com",
}
privacyProfile := msgraphsdk.NewPrivacyProfile()
requestBody.SetPrivacyProfile(privacyProfile)
contactEmail := "alice@contoso.com"
privacyProfile.SetContactEmail(&contactEmail)
statementUrl := "https://contoso.com/privacyStatement"
privacyProfile.SetStatementUrl(&statementUrl)
requestBody.SetSecurityComplianceNotificationMails( []String {
    "security@contoso.com",
}
requestBody.SetSecurityComplianceNotificationPhones( []String {
    "(123) 456-7890",
}
requestBody.SetTechnicalNotificationMails( []String {
    "tech@contoso.com",
}
options := &msgraphsdk.OrganizationRequestBuilderPatchOptions{
    Body: requestBody,
}
organizationId := "organization-id"
result, err := graphClient.OrganizationById(&organizationId).Patch(options)


```