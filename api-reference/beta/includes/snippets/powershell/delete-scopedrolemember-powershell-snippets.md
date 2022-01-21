---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6112c0931a434f0d0d2ee06cee084b4d0fd8f6a2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116932"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Remove-MgAdministrativeUnitScopedRoleMember -AdministrativeUnitId $administrativeUnitId -ScopedRoleMembershipId $scopedRoleMembershipId

```