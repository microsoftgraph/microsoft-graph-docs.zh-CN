---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 63754df4bb09348a1c25fe3ca47d0c5d0baf72c2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859667"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("startdatetime", "{start_datetime}"),
    new QueryOption("enddatetime", "{end_datetime}")
};

var delta = await graphClient.Me.CalendarView
    .Delta()
    .Request( queryOptions )
    .GetAsync();

```