---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5b3174df4b16176050a41ce14552cd25daaf280
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66040954"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgDirectoryAdministrativeUnitMemberByRef -AdministrativeUnitId $administrativeUnitId

```