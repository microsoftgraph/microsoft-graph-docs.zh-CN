---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69ac025ad1f7b86e1b2da49dbccacbea8f7c5c67
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806495"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("startDateTime", "2020-06-01T00:00:00Z"),
    new QueryOption("endDateTime", "2020-06-10T00:00:00Z")
};

var delta = await graphClient.Me.Calendars["{calendar-id}"].CalendarView
    .Delta()
    .Request( queryOptions )
    .GetAsync();

```