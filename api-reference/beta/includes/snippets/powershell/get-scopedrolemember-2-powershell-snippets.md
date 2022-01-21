---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7085cc069f633cbca96b3bc3f43e398a35e49f6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62110056"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgAdministrativeUnitScopedRoleMember -AdministrativeUnitId $administrativeUnitId

```