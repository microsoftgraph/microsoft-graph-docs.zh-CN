---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cc5b5fa6e7eb2c0a83e4348e3107fcfca03f664
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351120"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Get-MgUserMessage -UserId $userId -MessageId $messageId -ExpandProperty "singleValueExtendedProperties(`$filter=id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color')" 

```