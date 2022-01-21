---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3827d4791c7bd37d39f48f41c8a33094fcabc516
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62102166"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgUserAuthenticationTemporaryAccessPassMethod -UserId $userId

```