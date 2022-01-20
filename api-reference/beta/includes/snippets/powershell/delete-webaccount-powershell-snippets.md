---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f19f820606207a6ed769362b1636a1fc0c1f90cd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62092695"
---
```powershell

Import-Module Microsoft.Graph.People

Remove-MgUserProfileWebAccount -UserId $userId -WebAccountId $webAccountId

```