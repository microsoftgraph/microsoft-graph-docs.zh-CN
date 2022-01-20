---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a8bf6221aa3c6a5cbd0b1d08789a6d5d65c4f75
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133614"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgUserAuthenticationEmailMethod -UserId $userId

```