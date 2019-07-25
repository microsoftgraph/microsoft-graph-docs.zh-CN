---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a79bd1d35a9525c20b98d5472fb8f489bd1b1ba9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866660"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailboxSettings = new MailboxSettings
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.context","https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings"}
    },
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
    }
};

var me = new User();
me.MailboxSettings = mailboxSettings;

await graphClient.Me
    .Request()
    .UpdateAsync(me);

```