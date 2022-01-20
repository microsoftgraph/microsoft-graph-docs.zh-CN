---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bec48c87e548c32298fc9bea225b6c1f7d9fbf04
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095417"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgDirectoryAdministrativeUnitScopedRoleMember -AdministrativeUnitId $administrativeUnitId -ScopedRoleMembershipId $scopedRoleMembershipId

```