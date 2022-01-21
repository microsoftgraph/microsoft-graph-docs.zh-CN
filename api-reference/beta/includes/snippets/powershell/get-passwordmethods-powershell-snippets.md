---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fc2cfd310341360183535f8b7671d7dc8de400c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116792"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgUserAuthenticationPasswordMethod -UserId $userId

```