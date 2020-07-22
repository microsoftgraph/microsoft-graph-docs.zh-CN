---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5df8fd123222cc6e6e8c028fd56a16d5f6c295f5
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2020
ms.locfileid: "45224724"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onlineMeeting = new OnlineMeeting
{
    StartDateTime = DateTimeOffset.Parse("2020-09-09T21:33:30.8546353+00:00"),
    EndDateTime = DateTimeOffset.Parse("2020-09-09T22:03:30.8566356+00:00"),
    Subject = "Patch Meeting Subject"
};

await graphClient.Me.OnlineMeetings["{id}"]
    .Request()
    .UpdateAsync(onlineMeeting);

```