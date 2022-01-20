---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bdd71880019940a4867a1e494987cfb9d8d72c1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135986"
---
```powershell

Import-Module Microsoft.Graph.Notes

$params = @{
    DisplayName = "Section name"
}

New-MgUserOnenoteNotebookSection -UserId $userId -NotebookId $notebookId -BodyParameter $params

```