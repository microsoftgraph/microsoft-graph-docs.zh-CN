---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b24cb54ce73dfc8e3cd5779c27b04ca17970380
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612973"
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

await graphClient.Me.MailFolders["inbox"].MessageRules
    .Request()
    .AddAsync(messageRule);

```