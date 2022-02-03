---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9967a4562c4314fb754156d009037dc38cfcc2da
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348003"
---
```powershell

Import-Module Microsoft.Graph.Users.Functions

# A UPN can also be used as -UserId.
Invoke-MgSupportedUserOutlookLanguage -UserId $userId

```