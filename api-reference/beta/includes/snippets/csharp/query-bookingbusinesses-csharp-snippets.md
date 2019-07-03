---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 25b878914d55d3a0b6152ae3c12c60c6db3a2673
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521222"
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