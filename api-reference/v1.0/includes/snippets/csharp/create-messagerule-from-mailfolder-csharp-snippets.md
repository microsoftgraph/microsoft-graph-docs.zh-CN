---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a93602cf57ec5c65929cf87c11d84a1e3d5b7b54
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789727"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messageRule = new MessageRule
{
    DisplayName = "From partner",
    Sequence = 2,
    IsEnabled = true,
    Conditions = new MessageRulePredicates
    {
        SenderContains = new List<String>()
        {
            "adele"
        }
    },
    Actions = new MessageRuleActions
    {
        ForwardTo = new List<Recipient>()
        {
            new Recipient
            {
                EmailAddress = new EmailAddress
                {
                    Name = "Alex Wilbur",
                    Address = "AlexW@contoso.onmicrosoft.com"
                }
            }
        },
        StopProcessingRules = true
    }
};

await graphClient.Me.MailFolders["{mailFolder-id}"].MessageRules
    .Request()
    .AddAsync(messageRule);

```