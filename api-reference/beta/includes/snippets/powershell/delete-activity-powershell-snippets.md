---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 088decec2c2000e349a86d4bb6113f385c074b22
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349622"
---
```powershell

Import-Module Microsoft.Graph.CrossDeviceExperiences

# A UPN can also be used as -UserId.
Remove-MgUserActivity -UserId $userId -UserActivityId $userActivityId

```