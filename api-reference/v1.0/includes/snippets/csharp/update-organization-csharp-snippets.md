---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ece37c53f1e271cbc48d0d4a46535b26b08144a2
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618865"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organization = new Organization
{
    MarketingNotificationEmails = new List<String>()
    {
        "marketing@contoso.com"
    },
    PrivacyProfile = new PrivacyProfile
    {
        ContactEmail = "alice@contoso.com",
        StatementUrl = "https://contoso.com/privacyStatement"
    },
    SecurityComplianceNotificationMails = new List<String>()
    {
        "security@contoso.com"
    },
    SecurityComplianceNotificationPhones = new List<String>()
    {
        "(123) 456-7890"
    },
    TechnicalNotificationMails = new List<String>()
    {
        "tech@contoso.com"
    }
};

await graphClient.Organization["{id}"]
    .Request()
    .UpdateAsync(organization);

```