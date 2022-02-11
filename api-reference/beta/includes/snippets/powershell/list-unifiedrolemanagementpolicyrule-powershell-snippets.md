---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 809555be162f3b3de3de728521044b168cfc42da
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62530527"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgPolicyRoleManagementPolicyEffectiveRule -UnifiedRoleManagementPolicyId $unifiedRoleManagementPolicyId

```