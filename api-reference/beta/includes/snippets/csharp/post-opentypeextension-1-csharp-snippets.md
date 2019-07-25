---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 04230414b68d1fde64016bc08524006fc40db2e7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878352"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    Subject = "Annual review",
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "You should be proud!"
    },
    ToRecipients = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Address = "rufus@contoso.com"
            }
        }
    },
    Extensions = new List<Extension>()
    {
        new Extension
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"@odata.type","microsoft.graph.openTypeExtension"}
            },
            ExtensionName = "Com.Contoso.Referral",
            CompanyName = "Wingtip Toys",
            ExpirationDate = "2015-12-30T11:00:00Z",
            DealValue = 10000
        }
    }
};

await graphClient.Me.Messages
    .Request()
    .AddAsync(message);

```