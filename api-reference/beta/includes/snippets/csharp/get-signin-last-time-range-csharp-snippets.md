---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c242f19811f70ff2718c35777b35b002e5cee9a2
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947173"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("filter", "signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z")
};

var users = await graphClient.Users
    .Request( queryOptions )
    .Filter("signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z")
    .GetAsync();

```