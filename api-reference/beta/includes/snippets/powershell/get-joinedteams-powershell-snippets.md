---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1e9a837edd8405e232fdb6e0bfc124ebd7f0f99
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352023"
---
```powershell

Import-Module Microsoft.Graph.Teams

# A UPN can also be used as -UserId.
Get-MgUserJoinedTeam -UserId $userId

```