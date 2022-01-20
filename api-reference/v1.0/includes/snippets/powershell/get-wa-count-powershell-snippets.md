---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8bbb99b86413989a9cdc6e726d476fb5446b687d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100787"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUser -Search "displayName:wa" -Sort "displayName" -CountVariable CountVar -ConsistencyLevel eventual 


```