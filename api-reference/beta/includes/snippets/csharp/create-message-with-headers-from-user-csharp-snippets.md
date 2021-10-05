---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4751832f7adee345202e533772e8dc28b1ab262d386829a80a4d2966f5bd673d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215763"
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