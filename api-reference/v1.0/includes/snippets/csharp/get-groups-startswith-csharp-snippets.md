---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc6b07cb321808d0c669b86cb651db793ae43670
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209987"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var groups = await graphClient.Groups
    .Request( queryOptions )
    .Header("ConsistencyLevel","eventual")
    .Filter("startswith(displayName, 'a')")
    .OrderBy("displayName")
    .Top(1)
    .GetAsync();

```