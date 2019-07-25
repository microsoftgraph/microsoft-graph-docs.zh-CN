---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 979cdb95e2ca624079bf71bd5072c54809c1c344
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716390"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    Subject = "9/8/2018: concert",
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "The group represents Washington."
    },
    ToRecipients = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Address = "AlexW@contoso.OnMicrosoft.com"
            }
        }
    },
    InternetMessageHeaders = new List<InternetMessageHeader>()
    {
        new InternetMessageHeader
        {
            Name = "x-custom-header-group-name",
            Value = "Washington"
        },
        new InternetMessageHeader
        {
            Name = "x-custom-header-group-id",
            Value = "WA001"
        }
    }
};

await graphClient.Me.Messages
    .Request()
    .AddAsync(message);

```