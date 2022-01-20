---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b051ad1971e8abf375f39348655cac4c0c07bda
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132627"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgPolicyRoleManagementPolicyRule -UnifiedRoleManagementPolicyId $unifiedRoleManagementPolicyId -UnifiedRoleManagementPolicyRuleId $unifiedRoleManagementPolicyRuleId

```