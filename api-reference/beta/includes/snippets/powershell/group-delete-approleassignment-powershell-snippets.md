---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49290a97ef306cb6489f02c322d0f5dc92ab7714
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133600"
---
```powershell

Import-Module Microsoft.Graph.Applications

Remove-MgGroupAppRoleAssignment -GroupId $groupId -AppRoleAssignmentId $appRoleAssignmentId

```