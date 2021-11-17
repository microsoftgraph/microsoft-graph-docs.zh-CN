---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 73f997acfdae3c31a6ccad3f93f3dc4223380a5dc8398267c38f22f72d552c0e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162395"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "I won't be able to make this week. How about next week?";

var sendResponse = true;

var proposedNewTime = new TimeSlot
{
    Start = new DateTimeTimeZone
    {
        DateTime = "2019-12-02T18:00:00",
        TimeZone = "Pacific Standard Time"
    },
    End = new DateTimeTimeZone
    {
        DateTime = "2019-12-02T19:00:00",
        TimeZone = "Pacific Standard Time"
    }
};

await graphClient.Me.Events["{event-id}"]
    .Decline(comment,sendResponse,proposedNewTime)
    .Request()
    .PostAsync();

```