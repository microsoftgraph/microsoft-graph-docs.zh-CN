---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd9869eabe17159cfc955baf63ce33a6abf8b890
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62108648"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgUserAuthenticationPasswordMethod -UserId $userId -PasswordAuthenticationMethodId $passwordAuthenticationMethodId

```