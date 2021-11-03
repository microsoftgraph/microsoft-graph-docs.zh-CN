---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39b78f086aa2c3e18d0f1c6ea8edd30e42e2a34d450b0b4c8045521179fcf3dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105835"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("start", "2018-04-30T00:00:00Z"),
    new QueryOption("end", "2018-05-10T00:00:00Z")
};

var calendarView = await graphClient.BookingBusinesses["{bookingBusiness-id}"].CalendarView
    .Request( queryOptions )
    .GetAsync();

```