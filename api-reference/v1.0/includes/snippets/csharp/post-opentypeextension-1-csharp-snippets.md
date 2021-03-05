---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e71de90e4dd8ec67e895c788901c35c969d8c9a
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470869"
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