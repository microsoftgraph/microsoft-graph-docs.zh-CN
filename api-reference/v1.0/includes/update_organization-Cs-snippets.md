---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ece37c53f1e271cbc48d0d4a46535b26b08144a2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462360"
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