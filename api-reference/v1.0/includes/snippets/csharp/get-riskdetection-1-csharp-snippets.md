---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12ec01f1f30c21056665b9c67bed98f41127cf0f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088233"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskDetection = await graphClient.IdentityProtection.RiskDetections["{riskDetection-id}"]
    .Request()
    .GetAsync();

```