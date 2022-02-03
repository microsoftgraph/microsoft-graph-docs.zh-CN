---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 306d002f3e86c4aa9467db6d9e0d81aacf3cc9a9
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351667"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfilePhone -UserId $userId -ItemPhoneId $itemPhoneId

```