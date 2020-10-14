---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5426851811296d1449613826e0d7bb2ae7bfbd45
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48462652"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var set = new Microsoft.Graph.TermStore.Set
{
    Description = "mySet"
};

await graphClient.TermStore.Sets["{setId}"]
    .Request()
    .UpdateAsync(set);

```