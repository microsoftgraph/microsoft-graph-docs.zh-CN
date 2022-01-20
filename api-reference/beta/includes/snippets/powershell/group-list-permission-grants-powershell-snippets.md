---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 170028d42c5b25d88db93c46358c8bae1c70c2d8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131234"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroupPermissionGrant -GroupId $groupId

```