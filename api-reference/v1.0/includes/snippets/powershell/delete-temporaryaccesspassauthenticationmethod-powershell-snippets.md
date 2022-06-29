---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 441f7a75375b2f14bd99ff37d2def4a26d736cd8
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444411"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgUserAuthenticationTemporaryAccessPassMethod -UserId $userId -TemporaryAccessPassAuthenticationMethodId $temporaryAccessPassAuthenticationMethodId

```