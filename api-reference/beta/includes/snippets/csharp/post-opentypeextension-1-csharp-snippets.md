---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 628fd2acddf8f84bac0e5cf11031fbfe3d71145e1e7cb45083d63b9f8bd4de14
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279140"
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
    Extensions = new MessageExtensionsCollectionPage()
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