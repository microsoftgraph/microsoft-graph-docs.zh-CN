---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8572efd109a81d9a880ccc06d055dad4f7e428c5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136778"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgUserAuthenticationWindowHello -UserId $userId -WindowsHelloForBusinessAuthenticationMethodId $windowsHelloForBusinessAuthenticationMethodId

```