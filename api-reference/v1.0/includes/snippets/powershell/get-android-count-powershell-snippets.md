---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8df30575c34a805bac45e3105e45867df754258
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62225515"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgDevice -Search "displayName:Android" -CountVariable CountVar -ConsistencyLevel eventual 


```