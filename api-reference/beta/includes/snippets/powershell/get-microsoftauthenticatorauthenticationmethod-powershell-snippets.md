---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f29f15411b44be14596e4883d48c8854d8d76e9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113076"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgUserAuthenticationMicrosoftAuthenticatorMethod -UserId $userId -MicrosoftAuthenticatorAuthenticationMethodId $microsoftAuthenticatorAuthenticationMethodId

```