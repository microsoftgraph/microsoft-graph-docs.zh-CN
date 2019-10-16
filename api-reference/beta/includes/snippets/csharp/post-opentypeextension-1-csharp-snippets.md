---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3be1198598a0533702ebfec8513afc7f2a11f6f
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544189"
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
        new OpenTypeExtension
        {
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