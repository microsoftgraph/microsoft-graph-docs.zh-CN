---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0852d1a97b7f27d76964f0bd6b9a166d03efaa35
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351258"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Remove-MgUserMessageMention -UserId $userId -MessageId $messageId -MentionId $mentionId

```