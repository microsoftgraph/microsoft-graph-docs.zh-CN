---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2b07454b385e23a204e4226c8c2dd51d09798c8008a293f40fc6a239b7e8eeb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220055"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    Subject = "9/9/2018: concert",
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "The group represents Nevada."
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
            Value = "Nevada"
        },
        new InternetMessageHeader
        {
            Name = "x-custom-header-group-id",
            Value = "NV001"
        }
    }
};

await graphClient.Me
    .SendMail(message,null)
    .Request()
    .PostAsync();

```