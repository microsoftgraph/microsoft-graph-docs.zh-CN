---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f73deb5b3b3c44d48b91df863e90a4e19e7eb615
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725752"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskDetections = await graphClient.RiskDetections
    .Request()
    .GetAsync();

```