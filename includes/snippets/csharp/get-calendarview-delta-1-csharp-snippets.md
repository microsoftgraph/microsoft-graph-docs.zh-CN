---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3766f4ff3db0355419476ecca0cd3b4fed722b9d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881160"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("startdatetime", "2016-12-01T00:00:00Z"),
    new QueryOption("enddatetime", "2016-12-30T00:00:00Z")
};

var delta = await graphClient.Me.CalendarView
    .Delta()
    .Request( queryOptions )
    .Header("Prefer","odata.maxpagesize=2")
    .GetAsync();

```