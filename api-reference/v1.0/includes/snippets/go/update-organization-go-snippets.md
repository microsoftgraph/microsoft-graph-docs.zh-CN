---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e4c467d3e0f4452683cc0aba34035ec954d0964
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027339"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
graphClient.OrganizationById(&organizationId).Patch(options)


```