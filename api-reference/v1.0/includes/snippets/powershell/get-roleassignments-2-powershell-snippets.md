---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 607fe37032dbefd8e0673fde212a54c82df177ef
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132222"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

Get-MgRoleManagementDirectoryRoleAssignment -Filter  " principalId eq 'f1847572-48aa-47aa-96a3-2ec61904f41f'" 

```