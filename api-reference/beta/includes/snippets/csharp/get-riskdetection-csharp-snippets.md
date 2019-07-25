---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b20a4679120ad135c216ed8c92f31b40387ca7a7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725791"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskDetection = await graphClient.RiskDetections["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
    .Request()
    .GetAsync();

```