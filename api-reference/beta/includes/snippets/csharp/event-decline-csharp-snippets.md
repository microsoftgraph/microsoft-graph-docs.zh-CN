---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 886346fb8eb527c56cf7dfa1136a8f6a89ae7d04
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992282"
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