---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b20a4679120ad135c216ed8c92f31b40387ca7a7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519577"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskDetection = await graphClient.RiskDetections["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
    .Request()
    .GetAsync();

```