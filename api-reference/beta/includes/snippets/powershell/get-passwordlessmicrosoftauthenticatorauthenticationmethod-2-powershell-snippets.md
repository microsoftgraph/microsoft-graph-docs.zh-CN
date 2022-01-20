---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81dc65a8e0e646a70f819243fe0ae71c7ceef502
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089543"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgUserAuthenticationPasswordlessMicrosoftAuthenticatorMethod -UserId $userId

```