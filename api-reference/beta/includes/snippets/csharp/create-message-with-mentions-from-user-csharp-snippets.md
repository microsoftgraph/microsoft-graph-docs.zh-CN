---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20133013df53990e84fa8dfe9d83956fe3be9a80
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945326"
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
    Mentions = new MessageMentionsCollectionPage()
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