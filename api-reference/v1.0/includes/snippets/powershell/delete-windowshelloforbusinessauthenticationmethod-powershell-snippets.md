---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 965d570184187d4e75db0d71184c795841e0f3f1
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66502422"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgUserAuthenticationWindowHelloForBusinessMethod -UserId $userId -WindowsHelloForBusinessAuthenticationMethodId $windowsHelloForBusinessAuthenticationMethodId

```