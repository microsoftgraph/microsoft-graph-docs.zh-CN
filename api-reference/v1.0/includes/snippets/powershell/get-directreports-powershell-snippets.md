---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7805c916d8dacf2b9ddb239d58c5b74d2fa17605
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351172"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Get-MgUserDirectReport -UserId $userId

```