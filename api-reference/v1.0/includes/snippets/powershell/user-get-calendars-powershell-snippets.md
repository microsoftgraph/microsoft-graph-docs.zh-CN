---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 087fed3340c02c15dddc2f93dba21816ae7fa170
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349285"
---
```powershell

Import-Module Microsoft.Graph.Calendar

# A UPN can also be used as -UserId.
Get-MgUserCalendar -UserId $userId

```