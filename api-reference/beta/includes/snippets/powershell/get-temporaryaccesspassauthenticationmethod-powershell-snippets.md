---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57c5e03b34c38fd74570875575c06b01d40f33a0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126796"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgUserAuthenticationTemporaryAccessPassMethod -UserId $userId -TemporaryAccessPassAuthenticationMethodId $temporaryAccessPassAuthenticationMethodId

```