---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18bd19de7e80eb0fd1dd27ab0f126c9bf1b9f8f6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130562"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Get-MgUserEvent -UserId $userId -Property "subject,body,bodyPreview,organizer,attendees,start,end,location" 

```