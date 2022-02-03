---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9c79518eec2b91dec198c6b409835873fd4e1f1
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350578"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Get-MgUserMessageExtension -UserId $userId -MessageId $messageId -ExtensionId $extensionId

```