---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bbf08baadbfa18643d439b17e986f51665fed39
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351912"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileCertification -UserId $userId

```