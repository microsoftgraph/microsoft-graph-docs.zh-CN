---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9a22ecd2327c75c63aab21ce670fec3561f7d95
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62225629"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroupTransitiveMember -GroupId $groupId

```