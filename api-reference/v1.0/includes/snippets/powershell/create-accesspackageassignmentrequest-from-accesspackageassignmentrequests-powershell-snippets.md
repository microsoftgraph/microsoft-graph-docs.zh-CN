---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d2fbf002e5bf3c1234a65621f3369bc38b635cb
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220298"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    RequestType = "userAdd"
    Assignment = @{
        AccessPackageId = "d7be3253-b9c6-4fab-adef-30d30de8da2b"
    }
}

New-MgEntitlementManagementAssignmentRequest -BodyParameter $params

```