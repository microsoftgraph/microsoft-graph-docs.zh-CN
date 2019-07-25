---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5719b9988ae5e350728d62dd2ccf7112872957cc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709761"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("start", "2018-04-30T00:00:00Z"),
    new QueryOption("end", "2018-05-10T00:00:00Z")
};

var calendarView = await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].CalendarView
    .Request( queryOptions )
    .GetAsync();

```