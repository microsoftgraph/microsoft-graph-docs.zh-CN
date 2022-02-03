---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3261e93bb3fc93ef832e049d69c1e9888a38fe7b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352772"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

# A UPN can also be used as -UserId.
Get-MgUserAuthenticationTemporaryAccessPassMethod -UserId $userId

```