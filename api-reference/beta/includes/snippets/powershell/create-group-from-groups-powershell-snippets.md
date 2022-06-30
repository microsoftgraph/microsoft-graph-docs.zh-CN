---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d24f96cd3be5b92acb97fc1e91ec1f360f2253c
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443326"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    "@odata.id" = "https://graph.microsoft.com/odata/groups('1a9db3ab-0acf-4808-99ae-e8ed581cb2e0')"
}

New-MgPolicyMobileAppManagementPolicyIncludedGroupByRef -MobilityManagementPolicyId $mobilityManagementPolicyId -BodyParameter $params

```