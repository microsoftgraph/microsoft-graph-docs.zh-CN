---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e98a50351162b44c8ce22666f6d54bed64948897
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66040959"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgDirectoryAdministrativeUnitMember -AdministrativeUnitId $administrativeUnitId

```