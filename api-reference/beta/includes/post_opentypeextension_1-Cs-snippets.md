---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 44643064b53829741042a604fb082ab2e9575681
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34546647"
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