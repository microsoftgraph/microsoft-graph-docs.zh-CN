---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f041da5de1561b048620500df777d2850ad0f59e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211662"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroupMember -GroupId $groupId -CountVariable CountVar -Filter "startswith(displayName, 'a')" 

```