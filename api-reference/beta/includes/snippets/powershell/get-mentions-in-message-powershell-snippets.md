---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1c83f6ef866f51a7821b32723b46450ecd3609a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099507"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMessage -UserId $userId -MessageId $messageId -ExpandProperty "mentions" 

```