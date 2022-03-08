---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f099f666e5bd066989009530ec9fe5cd4ac2a74a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336660"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var user = await graphClient.Me
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Expand("manager($levels=max;$select=id,displayName)")
    .Select("id,displayName")
    .GetAsync();

```