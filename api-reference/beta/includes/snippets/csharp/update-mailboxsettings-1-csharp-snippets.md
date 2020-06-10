---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a5adffb34f211ff52da38f635c78969fdbb8613
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684621"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailboxSettings = new MailboxSettings
{
    AutomaticRepliesSetting = new AutomaticRepliesSetting
    {
        Status = AutomaticRepliesStatus.Scheduled,
        ScheduledStartDateTime = new DateTimeTimeZone
        {
            DateTime = "2016-03-20T18:00:00",
            TimeZone = "UTC"
        },
        ScheduledEndDateTime = new DateTimeTimeZone
        {
            DateTime = "2016-03-28T18:00:00",
            TimeZone = "UTC"
        }
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.context", "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings"}
    }
};

var me = new User();
me.MailboxSettings = mailboxSettings;

await graphClient.Me
    .Request()
    .UpdateAsync(me);

```