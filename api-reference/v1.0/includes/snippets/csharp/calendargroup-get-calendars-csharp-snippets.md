---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51b18affb6b55059f438a2c715a8436cf30d47082c0e61b2264de025f7edc5be
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332135"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendars = await graphClient.Me.CalendarGroups["{calendarGroup-id}"].Calendars
    .Request()
    .GetAsync();

```