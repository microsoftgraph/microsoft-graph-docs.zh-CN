---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1890e89a1e565c8533333ff394daeebaaa621d12
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129601"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Get-MgPrivilegedRoleRoleAssignment -Filter "isElevated eq true" 

```