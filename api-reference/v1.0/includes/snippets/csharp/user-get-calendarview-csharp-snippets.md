---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f1429a19dc2beeef4c36370146099bfd4083a78
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2020
ms.locfileid: "41123113"
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