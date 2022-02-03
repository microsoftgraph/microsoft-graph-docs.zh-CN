---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6aa21916902c20575d3303868c4f768149b45f38
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350728"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

# A UPN can also be used as -UserId.
Get-MgUserContact -UserId $userId -Property "displayName,emailAddresses" 

```