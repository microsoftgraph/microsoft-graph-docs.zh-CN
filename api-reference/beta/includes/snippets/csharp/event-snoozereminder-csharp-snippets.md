---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee8ae3d3c7f28a9d26223819fe4f197f365412f1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804183"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var newReminderTime = new DateTimeTimeZone
{
    DateTime = "2016-10-19T10:37:00Z",
    TimeZone = "timeZone-value"
};

await graphClient.Me.Events["{event-id}"]
    .SnoozeReminder(newReminderTime)
    .Request()
    .PostAsync();

```