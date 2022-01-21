---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ebef26cafef10e6cbfe0a2ca97fe43fd1c5ad60
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129225"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Remove-MgDirectoryAdministrativeUnitScopedRoleMember -AdministrativeUnitId $administrativeUnitId -ScopedRoleMembershipId $scopedRoleMembershipId

```