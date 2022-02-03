---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8cbd1d31b577fbbdcdf698692b557686b1a84912
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350039"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserUsedInsight -UserId $userId -Sort "LastUsed/LastAccessedDateTime desc" 

```