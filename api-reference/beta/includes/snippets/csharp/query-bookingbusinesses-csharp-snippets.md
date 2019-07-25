---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 25b878914d55d3a0b6152ae3c12c60c6db3a2673
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709872"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("query", "Adventure")
};

var bookingBusinesses = await graphClient.BookingBusinesses
    .Request( queryOptions )
    .GetAsync();

```