---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4cefb68f5c29ca89cb2d051dbdceed1a4d27d539ca4b301b505fe418fcdaeca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903153"
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