---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7faf34a1dcfc9465192630ff1cd06bdc8bd70108
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137176"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Get-MgPrivilegedAccessRoleSetting -PrivilegedAccessId $privilegedAccessId -GovernanceRoleSettingId $governanceRoleSettingId

```