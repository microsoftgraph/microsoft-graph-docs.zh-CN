---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 309e012419764a720e5d9fa93eed021d411c1b0e
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2019
ms.locfileid: "37636941"
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

await graphClient.Me.Events["{id}"]
    .Decline(proposedNewTime,sendResponse,comment)
    .Request()
    .PostAsync();

```