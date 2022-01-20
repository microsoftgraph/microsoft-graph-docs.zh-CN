---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b31d12594c4ecb5e463849602c5d726dc4db00b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125444"
---
```powershell

Import-Module Microsoft.Graph.Applications

Remove-MgServicePrincipalAppRoleAssignedTo -ServicePrincipalId $servicePrincipalId -AppRoleAssignmentId $appRoleAssignmentId

```