---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb2f0de89c5cb21672752282125dcf1d814738ce
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334784"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipalRiskDetections = await graphClient.IdentityProtection.ServicePrincipalRiskDetections
    .Request()
    .Filter("riskEventType eq 'investigationsThreatIntelligence' or riskLevel eq 'medium'")
    .GetAsync();

```