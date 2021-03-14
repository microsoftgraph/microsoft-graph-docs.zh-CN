---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bfe760ece1550ab31eccfe3ebc3240da86e93841
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796389"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var newReminderTime = new DateTimeTimeZone
{
    DateTime = "dateTime-value",
    TimeZone = "timeZone-value"
};

await graphClient.Me.Events["{event-id}"]
    .SnoozeReminder(newReminderTime)
    .Request()
    .PostAsync();

```