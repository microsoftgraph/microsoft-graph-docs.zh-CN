---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cea98a2f8578068f4185ea783947cdde8120d341
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117551"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    RequestType = "AdminRemove"
    Assignment = @{
        Id = "a6bb6942-3ae1-4259-9908-0133aaee9377"
    }
}

New-MgEntitlementManagementAssignmentRequest -BodyParameter $params

```