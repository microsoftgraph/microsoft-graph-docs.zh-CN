---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d3346930f0cc37aa583e2ae5c99107f2b398754
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350410"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

# A UPN can also be used as -UserId.
Get-MgUserAuthenticationMethod -UserId $userId -AuthenticationMethodId $authenticationMethodId

```