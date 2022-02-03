---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abb51a000f94d07c9007540366294748afd3e531
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351615"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileSkill -UserId $userId

```