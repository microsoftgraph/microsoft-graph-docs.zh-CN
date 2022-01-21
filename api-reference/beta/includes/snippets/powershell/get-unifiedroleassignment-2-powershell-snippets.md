---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b38124c0db594b1319d5998b8afffe062682944
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130689"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

Get-MgRoleManagementDirectoryRoleAssignment -UnifiedRoleAssignmentId $unifiedRoleAssignmentId -ExpandProperty "roleDefinition,principal,directoryScope" 

```