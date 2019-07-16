---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a9d6fbf463e9399f42279892e5793a503631df86
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736915"
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