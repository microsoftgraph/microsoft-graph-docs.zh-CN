---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b643b6e470f74a87f7ef11eae91f0cca1ad4605e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220276"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    "@odata.type" = "#microsoft.graph.mobilityManagementPolicy"
    ComplianceUrl = "https://portal.uem.contoso.com/?portalAction=Compliance"
    DiscoveryUrl = "https://enrollment.uem.contoso.com/enrollmentserver/discovery.svc"
    TermsOfUseUrl = "https://portal.uem.contoso.com/TermsofUse.aspx"
}

Update-MgPolicyMobileDeviceManagementPolicy -MobilityManagementPolicyId $mobilityManagementPolicyId -BodyParameter $params

```