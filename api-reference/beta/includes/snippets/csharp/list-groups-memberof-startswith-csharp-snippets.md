---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74d92078e27fc2ed4ad221573fbcc02a2355b375
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209005"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var group = await graphClient.Groups["{group-id}"].MemberOf
    .Request( queryOptions )
    .Header("ConsistencyLevel","eventual")
    .Filter("startswith(displayName, 'A')")
    .OrderBy("displayName")
    .GetAsync();

```