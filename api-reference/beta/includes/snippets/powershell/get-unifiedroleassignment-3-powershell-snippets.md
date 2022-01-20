---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d8ea7ca0014d99778b3ac91722ab8c31e2df4bd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135024"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

Get-MgRoleManagementCloudPcRoleAssignment -UnifiedRoleAssignmentMultipleId $unifiedRoleAssignmentMultipleId -ExpandProperty "roleDefinition" 

```