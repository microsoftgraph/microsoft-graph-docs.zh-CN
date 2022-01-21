---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d089522b9af1657c84fb0f07ba07b142734528b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123400"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUserOutlookTaskAttachment -UserId $userId -OutlookTaskId $outlookTaskId

```