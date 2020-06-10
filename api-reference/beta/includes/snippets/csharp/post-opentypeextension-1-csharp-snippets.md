---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff315abca3216fffb7b6096ac0d99944fbc9ec72
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684603"
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
    Extensions = (IMessageExtensionsCollectionPage)new List<Extension>()
    {
        new OpenTypeExtension
        {
            ExtensionName = "Com.Contoso.Referral",
            AdditionalData = new Dictionary<string, object>()
            {
                {"companyName", "Wingtip Toys"},
                {"expirationDate", "2015-12-30T11:00:00Z"},
                {"dealValue", "10000"}
            }
        }
    }
};

await graphClient.Me.Messages
    .Request()
    .AddAsync(message);

```