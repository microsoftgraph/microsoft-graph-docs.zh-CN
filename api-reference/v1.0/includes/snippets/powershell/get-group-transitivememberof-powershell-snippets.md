---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a4a6ecf8cc024f49fb0e19d4d0681e68d4f7bf7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114825"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroupTransitiveMemberOf -GroupId $groupId

```