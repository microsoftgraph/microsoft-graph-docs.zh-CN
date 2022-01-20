---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 414e17308ef77687ddd1e1571b590f6930a00428
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62098315"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgUserScopedRoleMemberOf -UserId $userId

```