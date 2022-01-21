---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8300d0bf0e70f25af8412f8fe848b599921055f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129599"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Get-MgPrivilegedRoleRoleAssignment -Filter "isElevated eq true and expirationDateTime eq null" 

```