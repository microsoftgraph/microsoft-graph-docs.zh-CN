---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 840bdc0e1f86a058459abf4a4e4d2df07a6863fc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103531"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    RoleTemplateId = "fe930be7-5e62-47db-91af-98c3a49a38b1"
}

New-MgDirectoryRole -BodyParameter $params

```