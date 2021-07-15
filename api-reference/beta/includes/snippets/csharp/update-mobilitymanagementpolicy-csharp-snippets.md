---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bcb708ef7276d67c05ff9289b70f06bf330f9353
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440345"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mobilityManagementPolicy = new MobilityManagementPolicy
{
    ComplianceUrl = "https://portal.uem.contoso.com/?portalAction=Compliance",
    DiscoveryUrl = "https://enrollment.uem.contoso.com/enrollmentserver/discovery.svc",
    TermsOfUseUrl = "https://portal.uem.contoso.com/TermsofUse.aspx"
};

await graphClient.Policies.MobileDeviceManagementPolicies["{mobilityManagementPolicy-id}"]
    .Request()
    .UpdateAsync(mobilityManagementPolicy);

```