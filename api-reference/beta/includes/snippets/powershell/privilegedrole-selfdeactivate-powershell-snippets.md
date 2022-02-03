---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8eb8f3fa2ce24ac2e0fe8c950e1174792ae3afff
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342966"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Invoke-MgSelfPrivilegedRoleDeactivate -PrivilegedRoleId $privilegedRoleId

```