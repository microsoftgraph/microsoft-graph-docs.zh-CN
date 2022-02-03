---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b6f6b076a7181e5732d31d8705a1d08e5e0fc86
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349299"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Get-MgUserOutlookMasterCategory -UserId $userId

```