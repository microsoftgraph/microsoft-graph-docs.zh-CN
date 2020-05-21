---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af965532fdbd637d61eefd3f5e0153a8616715a5
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332917"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var microsoft.graph.user = await graphClient.Groups["{id}"].Members.Microsoft.graph.user
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:Pr")
    .Select( e => new {
             e.DisplayName,
             e.Id 
             })
    .OrderBy("displayName ")
    .GetAsync();

```