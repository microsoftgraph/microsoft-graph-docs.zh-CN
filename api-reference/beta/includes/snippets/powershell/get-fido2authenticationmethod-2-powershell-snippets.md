---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b505394562cd35103ba5acbf30441ed082985017
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127852"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgUserAuthenticationFido2Method -UserId $userId

```