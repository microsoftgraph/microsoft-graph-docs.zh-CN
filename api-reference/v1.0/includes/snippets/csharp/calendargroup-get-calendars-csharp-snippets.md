---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b0a15c3a23b6b0a6acb30e8dcb782e1d17d0587
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804043"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendars = await graphClient.Me.CalendarGroups["{calendarGroup-id}"].Calendars
    .Request()
    .GetAsync();

```