---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df9979c87c60fcc820d421c6b71fa38b32b93acb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62110205"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    DisplayName = "Access Package New Name"
}

Update-MgEntitlementManagementAccessPackage -AccessPackageId $accessPackageId -BodyParameter $params

```