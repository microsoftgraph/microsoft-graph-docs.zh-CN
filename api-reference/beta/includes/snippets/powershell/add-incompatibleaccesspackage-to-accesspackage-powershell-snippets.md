---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2272f4056c5e61457a5c6a7b889cd7a9a5fab76f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107242"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    "@odata.id" = "https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2"
}

New-MgEntitlementManagementAccessPackageIncompatibleAccessPackageByRef -AccessPackageId $accessPackageId -BodyParameter $params

```