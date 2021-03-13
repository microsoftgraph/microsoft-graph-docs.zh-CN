---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c2a214d0189a948d692175e174d10cb0041d40f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791157"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTask = new OutlookTask
{
    DueDateTime = new DateTimeTimeZone
    {
        DateTime = "2016-05-06T16:00:00",
        TimeZone = "Eastern Standard Time"
    }
};

await graphClient.Me.Outlook.Tasks["{outlookTask-id}"]
    .Request()
    .Header("Prefer","outlook.timezone=\"Eastern Standard Time\"")
    .UpdateAsync(outlookTask);

```