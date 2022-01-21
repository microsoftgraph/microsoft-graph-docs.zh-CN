---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75ce601a6b38d28c011e98f806b45a115b3cf341
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123365"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUserOutlookTaskGroup -UserId $userId -OutlookTaskGroupId $outlookTaskGroupId

```