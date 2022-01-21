---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e98ccf3fd375268302a291330f60f04023282483
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126256"
---
```powershell

Import-Module Microsoft.Graph.Notes

Get-MgUserOnenoteNotebookSection -UserId $userId -NotebookId $notebookId

```