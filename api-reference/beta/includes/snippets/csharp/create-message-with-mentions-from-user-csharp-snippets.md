---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6ae45bca3d57bb715945b2acc93fd3efe60b275
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683809"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    Subject = "Party planning",
    ToRecipients = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Name = "Samantha Booth",
                Address = "samanthab@contoso.onmicrosoft.com"
            }
        }
    },
    Mentions = (IMessageMentionsCollectionPage)new List<Mention>()
    {
        new Mention
        {
            Mentioned = new EmailAddress
            {
                Name = "Dana Swope",
                Address = "danas@contoso.onmicrosoft.com"
            }
        }
    }
};

await graphClient.Me.Messages
    .Request()
    .AddAsync(message);

```