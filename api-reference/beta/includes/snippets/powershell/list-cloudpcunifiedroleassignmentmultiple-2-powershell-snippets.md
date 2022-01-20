---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9b11af325f7855f28dee8bb932445b9f3c2b574
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123045"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

Get-MgRoleManagementCloudPcRoleAssignment -Filter "roleDefinitionId eq 'b5c08161-a7af-481c-ace2-a20a69a48fb1'" 

```