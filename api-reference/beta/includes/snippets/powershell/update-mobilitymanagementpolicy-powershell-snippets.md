---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c30f519c207fe4128321d9ab036fdeeb4cb90ef
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099380"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    "@odata.type" = "#microsoft.graph.mobilityManagementPolicy"
    ComplianceUrl = "https://portal.mg.contoso.com/?portalAction=Compliance"
    DiscoveryUrl = "https://enrollment.mg.contoso.com/enrollmentserver/discovery.svc"
    TermsOfUseUrl = "https://portal.mg.contoso.com/TermsofUse.aspx"
}

Update-MgPolicyMobileAppManagementPolicy -MobilityManagementPolicyId $mobilityManagementPolicyId -BodyParameter $params

```