---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b1b675229c7e6270aafe9ca4d50abdadf4fac26a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133642"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgUserAuthenticationEmailMethod -UserId $userId -EmailAuthenticationMethodId $emailAuthenticationMethodId

```