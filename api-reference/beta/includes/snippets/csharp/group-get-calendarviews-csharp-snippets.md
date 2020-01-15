---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91c40964f2c19d01aed4231b4daee816490886e4
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2020
ms.locfileid: "41123107"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("startDateTime", "2017-01-01T19:00:00-08:00"),
    new QueryOption("endDateTime", "2017-10-01T19:00:00.00-08:00")
};

var calendarView = await graphClient.Groups["02bd9fd6-8f93-4758-87c3-1fb73740a315"].CalendarView
    .Request( queryOptions )
    .Header("Prefer","outlook.body-content-type=\"text\"")
    .GetAsync();

```