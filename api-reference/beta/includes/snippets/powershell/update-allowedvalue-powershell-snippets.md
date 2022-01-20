---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a19ecbfae97ea64ac1f3364688964e1ea6a40e1a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103917"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    IsActive = "false"
}

Update-MgDirectoryCustomSecurityAttributeDefinitionAllowedValue -CustomSecurityAttributeDefinitionId $customSecurityAttributeDefinitionId -AllowedValueId $allowedValueId -BodyParameter $params

```