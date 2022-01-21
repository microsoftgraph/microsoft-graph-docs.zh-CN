---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89cf0f774c76de7ca5a2898dcf0fd215be0ffd59
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112564"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgUserAuthenticationPasswordlessMicrosoftAuthenticatorMethod -UserId $userId -PasswordlessMicrosoftAuthenticatorAuthenticationMethodId $passwordlessMicrosoftAuthenticatorAuthenticationMethodId

```