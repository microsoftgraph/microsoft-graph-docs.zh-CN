---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5b18395af985fd23437336ccb5148d01764b39c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62096884"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    Description = "Target completion date (YYYY/MM/DD)"
}

Update-MgDirectoryCustomSecurityAttributeDefinition -CustomSecurityAttributeDefinitionId $customSecurityAttributeDefinitionId -BodyParameter $params

```