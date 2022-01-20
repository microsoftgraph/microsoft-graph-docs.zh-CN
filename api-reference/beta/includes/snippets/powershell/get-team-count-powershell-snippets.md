---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1b8bc36bc7bbc33ce285d85858e8340715804c6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127042"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgServicePrincipal -Search "displayName:Team" -CountVariable CountVar -ConsistencyLevel eventual 


```