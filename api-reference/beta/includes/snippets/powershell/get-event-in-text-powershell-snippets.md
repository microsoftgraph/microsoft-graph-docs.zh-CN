---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b1bb36632721ba285f7bc16108b03b4293483bf
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103087"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Get-MgUserEvent -UserId $userId -EventId $eventId -Property "subject,body,bodyPreview" 

```