---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c08ed60eb235b9a2a38fc91c6e7f8fe97062c9b5
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63396285"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

Get-MgRoleManagementDirectoryTransitiveRoleAssignment -CountVariable CountVar -Filter "principalId eq '2c7936bc-3517-40f3-8eda-4806637b6516'" 

```