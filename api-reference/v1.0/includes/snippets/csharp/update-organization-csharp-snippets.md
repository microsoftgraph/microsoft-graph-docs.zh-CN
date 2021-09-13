---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53577bb15fb6381d8042ec11c1627f7f71d4ba7c7c8c895da4be28464d84d81b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332552"
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

await graphClient.Organization["{organization-id}"]
    .Request()
    .UpdateAsync(organization);

```