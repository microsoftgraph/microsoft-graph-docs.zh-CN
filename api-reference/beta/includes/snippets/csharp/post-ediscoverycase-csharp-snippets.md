---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2bfc43209e7a692bb82545ea9a1eb581465ca470
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093653"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @case = new Microsoft.Graph.Ediscovery.Case
{
    DisplayName = "My Case 1"
};

await graphClient.Compliance.Ediscovery.Cases
    .Request()
    .AddAsync(@case);

```