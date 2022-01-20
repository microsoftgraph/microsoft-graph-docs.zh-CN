---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c60c010ab372de4a0a2549c5432eba9ead311673
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089811"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUserOutlookTask -UserId $userId -OutlookTaskId $outlookTaskId

```