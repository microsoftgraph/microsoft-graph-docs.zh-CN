---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6b721dff0363727b25eb6585a063ef8d3b8b6d2
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2020
ms.locfileid: "41123117"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("startDateTime", "2017-01-01T19:00:00-08:00"),
    new QueryOption("endDateTime", "2017-01-07T19:00:00-08:00")
};

var calendarView = await graphClient.Me.Calendar.CalendarView
    .Request( queryOptions )
    .GetAsync();

```