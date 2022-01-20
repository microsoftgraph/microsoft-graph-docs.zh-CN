---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df1f3e00133fc0e958f5af976c9d4f2e9876f0bf
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114937"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Get-MgUserEventAttachment -UserId $userId -EventId $eventId

```