---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 528cd7c9674e3ef6e1a8e5069a2f35f83674ca89
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128651"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgUserAuthenticationMicrosoftAuthenticatorMethod -UserId $userId

```