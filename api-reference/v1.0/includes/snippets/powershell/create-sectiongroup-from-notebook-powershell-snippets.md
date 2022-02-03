---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 710edd4def353b26a4d531990b17a320fdbda35e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352439"
---
```powershell

Import-Module Microsoft.Graph.Notes

$params = @{
    DisplayName = "Section group name"
}

# A UPN can also be used as -UserId.
New-MgUserOnenoteNotebookSectionGroup -UserId $userId -NotebookId $notebookId -BodyParameter $params

```