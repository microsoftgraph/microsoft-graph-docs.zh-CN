---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f4c36d96bd79525530e877b84961574561ab47d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340797"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

# A UPN can also be used as -UserId.
New-MgUserMessageForward -UserId $userId -MessageId $messageId

```