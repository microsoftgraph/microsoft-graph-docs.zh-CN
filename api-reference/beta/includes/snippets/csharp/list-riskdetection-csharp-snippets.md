---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f73deb5b3b3c44d48b91df863e90a4e19e7eb615
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "35725752"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskDetections = await graphClient.RiskDetections
    .Request()
    .GetAsync();

```