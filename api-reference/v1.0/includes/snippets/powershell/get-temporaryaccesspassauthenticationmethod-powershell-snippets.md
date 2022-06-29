---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57c5e03b34c38fd74570875575c06b01d40f33a0
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441076"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgUserAuthenticationTemporaryAccessPassMethod -UserId $userId -TemporaryAccessPassAuthenticationMethodId $temporaryAccessPassAuthenticationMethodId

```