---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b94efb99bb4409c635ecac9520eccffe8f029db0
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44338828"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskDetections = await graphClient.RiskDetections
    .Request()
    .Filter("riskEventType eq 'unfamiliarFeatures' or riskLevel eq 'medium'")
    .GetAsync();

```