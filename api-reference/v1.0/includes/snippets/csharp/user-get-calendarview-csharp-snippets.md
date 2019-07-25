---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 531415f3ba547c531c9b3e5f94525e2ac3e15ed7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886034"
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