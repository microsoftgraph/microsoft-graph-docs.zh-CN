---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c242f19811f70ff2718c35777b35b002e5cee9a2
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905684"
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