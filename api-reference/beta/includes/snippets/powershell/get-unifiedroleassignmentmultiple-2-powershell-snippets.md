---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8044640a31db6713ff3b6da5b1a3d2bd1c7fd474
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135023"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

Get-MgRoleManagementDeviceManagementRoleAssignment -Filter  " principalIds/any(x:x eq '564ae70c-73d9-476b-820b-fb61eb7384b9')" 

```