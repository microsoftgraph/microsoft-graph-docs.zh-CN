---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d3a0141b231bfe5d07bc16168655e6c75cc28568968a8459467fbce64e94efa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163394"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTask = new OutlookTask
{
    Subject = "Shop for dinner",
    StartDateTime = new DateTimeTimeZone
    {
        DateTime = "2016-04-23T18:00:00",
        TimeZone = "Pacific Standard Time"
    },
    DueDateTime = new DateTimeTimeZone
    {
        DateTime = "2016-04-25T13:00:00",
        TimeZone = "Pacific Standard Time"
    }
};

await graphClient.Me.Outlook.TaskFolders["{outlookTaskFolder-id}"].Tasks
    .Request()
    .AddAsync(outlookTask);

```