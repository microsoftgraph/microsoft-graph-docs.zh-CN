---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5aaab7d0a367e3a9e1ef281f5b1f27167302525
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122033"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskDetections = await graphClient.IdentityProtection.RiskDetections
    .Request()
    .GetAsync();

```