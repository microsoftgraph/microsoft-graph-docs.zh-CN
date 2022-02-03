---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce8b0c4418e71d253af0f7f355b7a10a47493080
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351219"
---
```powershell

Import-Module Microsoft.Graph.Notes

$params = @{
    DisplayName = "Section name"
}

# A UPN can also be used as -UserId.
New-MgUserOnenoteNotebookSection -UserId $userId -NotebookId $notebookId -BodyParameter $params

```