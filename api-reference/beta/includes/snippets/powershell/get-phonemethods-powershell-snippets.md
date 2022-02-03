---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d84876b227877a4b23d1bed1c3276cd96d4f9f21
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350945"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

# A UPN can also be used as -UserId.
Get-MgUserAuthenticationPhoneMethod -UserId $userId

```