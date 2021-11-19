---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aeb8bf644d8fde42754d4fa2248092e5271aee29
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082587"
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
graphClient.OrganizationById(&organizationId).Patch(options)


```