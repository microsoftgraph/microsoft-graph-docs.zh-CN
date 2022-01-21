---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c04df0b90e83080958c61e0702f019707cbaa02f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107382"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUser -UserId $userId -ExpandProperty "manager(`$levels=max;`$select=id,displayName)" -Property "id,displayName" -CountVariable CountVar -ConsistencyLevel eventual 


```