---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96b795b9a90a7436f6e5ee706c1ca9bf408bb563
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342777"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

# A UPN can also be used as -UserId.
New-MgUserMessageReply -UserId $userId -MessageId $messageId

```