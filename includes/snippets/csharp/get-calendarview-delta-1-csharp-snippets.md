---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dfb148d12475e83e3b4217648ba51f468b65c1c6fc212c7c786553aa440aa838
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54177837"
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