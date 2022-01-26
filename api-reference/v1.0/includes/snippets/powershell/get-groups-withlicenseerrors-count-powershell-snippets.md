---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e4bdfcf4d7291c64c5401c50d48225075c10317
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62225603"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroup -CountVariable CountVar -Filter "hasMembersWithLicenseErrors eq true" -Property "id,displayName" -ConsistencyLevel eventual 


```