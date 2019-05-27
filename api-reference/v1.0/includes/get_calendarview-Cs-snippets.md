---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 16b59d90d94be2a6cdffb203bf1c8c537e0f787d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457008"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarView = await graphClient.Me.CalendarView
    .Request()
    .GetAsync();

```