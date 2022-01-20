---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd60568826d269091133b8da21619aa3bd812e69
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116863"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    Description = "Attributes for engineering team"
    MaxAttributesPerSet = 20
}

Update-MgDirectoryAttributeSet -AttributeSetId $attributeSetId -BodyParameter $params

```