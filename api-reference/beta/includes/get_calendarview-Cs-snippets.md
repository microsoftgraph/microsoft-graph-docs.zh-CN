---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 531415f3ba547c531c9b3e5f94525e2ac3e15ed7
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536027"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("startDateTime", "2016-01-01T19:00:00.0000000"),
    new QueryOption("endDateTime", "2016-10-01T19:00:00.0000000")
};

var calendarView = await graphClient.Me.CalendarView
    .Request( queryOptions )
    .GetAsync();

```