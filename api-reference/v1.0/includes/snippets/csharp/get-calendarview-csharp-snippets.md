---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 531415f3ba547c531c9b3e5f94525e2ac3e15ed7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722039"
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