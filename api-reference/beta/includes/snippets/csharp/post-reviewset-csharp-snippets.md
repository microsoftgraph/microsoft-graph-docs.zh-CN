---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c96e41f65b4e7e9fc5767bbd689d1140d05a63b9
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093610"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reviewSet = new Microsoft.Graph.Ediscovery.ReviewSet
{
    DisplayName = "My Reviewset 3"
};

await graphClient.Compliance.Ediscovery.Cases["6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d"].ReviewSets
    .Request()
    .AddAsync(reviewSet);

```