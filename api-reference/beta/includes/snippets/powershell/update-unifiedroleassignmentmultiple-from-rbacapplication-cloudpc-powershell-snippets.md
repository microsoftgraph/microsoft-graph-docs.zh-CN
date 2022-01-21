---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a41afe3e564e0098113fdfd2c6bf128e7217ce20
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62105143"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

$params = @{
    DisplayName = "NewName"
    Description = "A new roleAssignment"
}

Update-MgRoleManagementCloudPcRoleAssignment -UnifiedRoleAssignmentMultipleId $unifiedRoleAssignmentMultipleId -BodyParameter $params

```