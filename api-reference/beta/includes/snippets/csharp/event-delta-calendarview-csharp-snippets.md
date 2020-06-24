---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80c46fad001331ee856ab376dc75ba25f313286a
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44862512"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("startDateTime", "2020-06-01T00:00:00Z"),
    new QueryOption("endDateTime", "2020-06-10T00:00:00Z")
};

var delta = await graphClient.Me.Calendars["AAMkADI5M1BbeAAA="].CalendarView
    .Delta()
    .Request( queryOptions )
    .GetAsync();

```