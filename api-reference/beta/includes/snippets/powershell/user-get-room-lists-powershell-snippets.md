---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dee0f699b5a86823b102fa993097bf5c1b78e702
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346446"
---
```powershell

Import-Module Microsoft.Graph.Users.Functions

# A UPN can also be used as -UserId.
Find-MgUserRoomList -UserId $userId

```