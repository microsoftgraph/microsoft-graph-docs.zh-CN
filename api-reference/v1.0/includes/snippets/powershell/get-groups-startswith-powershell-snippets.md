---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0123c305cc9fd160952728a256765d2d78f9416
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209982"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroup -Filter "startswith(displayName, 'a')" -CountVariable CountVar -Top 1 -Sort "displayName" -ConsistencyLevel eventual 


```