---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e17a0d23d2bad5548ed01caadd52f28588a4500b
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337276"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipalRiskDetection = await graphClient.IdentityProtection.ServicePrincipalRiskDetections["{servicePrincipalRiskDetection-id}"]
    .Request()
    .GetAsync();

```