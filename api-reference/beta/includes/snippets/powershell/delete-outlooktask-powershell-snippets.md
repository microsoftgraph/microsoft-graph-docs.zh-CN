---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a3a4d1920e8bac688c1ab2443f6b212c58df940
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123428"
---
```powershell

Import-Module Microsoft.Graph.Users

Remove-MgUserOutlookTask -UserId $userId -OutlookTaskId $outlookTaskId

```