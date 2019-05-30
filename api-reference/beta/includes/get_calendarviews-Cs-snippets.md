---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 780b00df0db836c20dc98d4ff8ce0bb81fc32cd3
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536006"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("startDateTime", "2017-01-01T19:00:00.0000000"),
    new QueryOption("endDateTime", "2017-10-01T19:00:00.00")
};

var calendarView = await graphClient.Groups["02bd9fd6-8f93-4758-87c3-1fb73740a315"].CalendarView
    .Request( queryOptions )
    .Header("Prefer","outlook.body-content-type=\"text\"")
    .GetAsync();

```