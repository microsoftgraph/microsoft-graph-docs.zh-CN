---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c00c0b4028266318c5ae4668830bf11f1597eb93
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62104546"
---
```powershell

Import-Module Microsoft.Graph.CrossDeviceExperiences

Remove-MgUserActivity -UserId $userId -UserActivityId $userActivityId

```