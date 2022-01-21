---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60a45f801a0fbaf9f76dcfe78e14987af0c613d3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62110450"
---
```powershell

Import-Module Microsoft.Graph.Applications

Remove-MgUserAppRoleAssignment -UserId $userId -AppRoleAssignmentId $appRoleAssignmentId

```