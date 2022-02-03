---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3285db8f3f7ef9f82d005614a6421eecdd8be78d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341531"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Id = "id-value"
    GroupId = "groupId-value"
    RenameAs = "renameAs-value"
}

# A UPN can also be used as -UserId.
Copy-MgUserOnenoteSectionToNotebook -UserId $userId -OnenoteSectionId $onenoteSectionId -BodyParameter $params

```