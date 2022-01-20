---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02c9c7b5f77cbb28ce1c3eecb22eab634c03d42d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133193"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgUserAuthenticationPasswordlessMicrosoftAuthenticatorMethod -UserId $userId -PasswordlessMicrosoftAuthenticatorAuthenticationMethodId $passwordlessMicrosoftAuthenticatorAuthenticationMethodId

```