---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8ae2e6affb3c58a4e617de2617fe91e0eb253b5
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347527"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Id = "id-value"
    GroupId = "groupId-value"
    RenameAs = "renameAs-value"
}

# A UPN can also be used as -UserId.
Copy-MgUserOnenoteSectionToSectionGroup -UserId $userId -OnenoteSectionId $onenoteSectionId -BodyParameter $params

```