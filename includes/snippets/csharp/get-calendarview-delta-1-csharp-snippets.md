---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a9d6fbf463e9399f42279892e5793a503631df86
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35533291"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("startdatetime", "2016-12-01T00:00:00Z"),
    new QueryOption("enddatetime", "2016-12-30T00:00:00Z")
};

var delta = await graphClient.Me.CalendarView.Delta()
    .Request( queryOptions )
    .Header("Prefer","odata.maxpagesize=2")
    .GetAsync();

```