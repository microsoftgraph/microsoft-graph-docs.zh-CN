---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ddfb0f549fb6cc9c6bfa16917e8867cd584ef31
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116807"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgUserAuthenticationSoftwareOathMethod -UserId $userId

```