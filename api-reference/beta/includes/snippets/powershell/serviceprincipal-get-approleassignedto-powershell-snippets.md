---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21986e0d46e4d64d28cd6afb0a533c237a03f7ea
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115826"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgServicePrincipalAppRoleAssignedTo -ServicePrincipalId $servicePrincipalId

```