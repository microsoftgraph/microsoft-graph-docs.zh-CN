---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82ab187470ce76d9e8ba92d7f25cab767dc725ae
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62108844"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgUserAuthenticationFido2Method -UserId $userId -Fido2AuthenticationMethodId $fido2AuthenticationMethodId

```