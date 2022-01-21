---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 028dddde8ed4374a2141c91eb66030df5a1aaaa6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124354"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgApplication -Search "displayName:Web" -CountVariable CountVar -ConsistencyLevel eventual 


```