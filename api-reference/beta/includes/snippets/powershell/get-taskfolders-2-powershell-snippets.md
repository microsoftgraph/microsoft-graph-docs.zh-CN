---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15ee4d5359632bb016676a1b5ed82b2c32dde1f1
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350779"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Get-MgUserOutlookTaskFolder -UserId $userId

```