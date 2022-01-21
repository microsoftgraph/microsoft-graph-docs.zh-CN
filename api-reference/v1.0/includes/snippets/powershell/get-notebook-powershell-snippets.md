---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55e9f21e9c5046b878c2dd0a9ea78dc266ef682c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128622"
---
```powershell

Import-Module Microsoft.Graph.Notes

Get-MgUserOnenoteNotebook -UserId $userId -NotebookId $notebookId

```