---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d225e38708dda38c58af848f5954ae68e00e0a73
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106311"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    Id = "Engineering"
    Description = "Attributes for engineering team"
    MaxAttributesPerSet = 25
}

New-MgDirectoryAttributeSet -BodyParameter $params

```