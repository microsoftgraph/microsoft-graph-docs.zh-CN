---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b3bcd34d5a3638d6b90bf910b42a10999f7955c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095204"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMessageContent -UserId $userId -MessageId $messageId

```