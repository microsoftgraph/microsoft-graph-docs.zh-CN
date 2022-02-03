---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f9c8f4639098be2e121cfe8259bcf34b84f1a70
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352730"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Remove-MgUserMessage -UserId $userId -MessageId $messageId

```