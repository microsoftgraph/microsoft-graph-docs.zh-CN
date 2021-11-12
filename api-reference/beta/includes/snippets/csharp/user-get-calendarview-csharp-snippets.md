---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9bc0e63bc5457c85d1539dc27291bea3800a33ecb3b30261754629b265e9ca5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106239"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("startDateTime", "2020-01-01T19:00:00-08:00"),
    new QueryOption("endDateTime", "2020-01-02T19:00:00-08:00")
};

var calendarView = await graphClient.Me.CalendarView
    .Request( queryOptions )
    .GetAsync();

```