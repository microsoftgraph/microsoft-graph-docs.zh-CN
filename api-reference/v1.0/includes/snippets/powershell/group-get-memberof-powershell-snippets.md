---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30fb7b54836726657512e01862b76f5794598eff
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114846"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroupMemberOf -GroupId $groupId

```