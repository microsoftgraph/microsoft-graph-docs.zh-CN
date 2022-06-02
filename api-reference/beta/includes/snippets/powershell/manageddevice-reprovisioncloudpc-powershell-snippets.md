---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69bed042e78ffc4597f3feeff65a6426d0882199
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65828763"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Actions

Invoke-MgReprovisionDeviceManagementManagedDeviceCloudPc -ManagedDeviceId $managedDeviceId

```