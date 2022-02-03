---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7907e672b97842353a2f9eb62efde6d2c677a567
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349628"
---
```powershell

Import-Module Microsoft.Graph.Notes

# A UPN can also be used as -UserId.
Get-MgUserOnenoteNotebookSection -UserId $userId -NotebookId $notebookId

```