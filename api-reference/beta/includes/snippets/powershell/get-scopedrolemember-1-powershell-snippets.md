---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b28c0932b0500b3ce1f07ceb21398bcc94e13a5f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114475"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgAdministrativeUnitScopedRoleMember -AdministrativeUnitId $administrativeUnitId -ScopedRoleMembershipId $scopedRoleMembershipId

```