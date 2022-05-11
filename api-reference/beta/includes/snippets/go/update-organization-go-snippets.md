---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7cb4e7f7a056616a4ac57f96b2bf6b7c02bbbca
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326899"
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
organizationId := "organization-id"
graphClient.OrganizationById(&organizationId).Patch(requestBody)


```