---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b28acd78e777a4e8507cb7f2f00a263f66f61f5b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089494"
---
```powershell

Import-Module Microsoft.Graph.Notes

$params = @{
    DisplayName = "Section name"
}

New-MgUserOnenoteSectionGroupSection -UserId $userId -SectionGroupId $sectionGroupId -BodyParameter $params

```