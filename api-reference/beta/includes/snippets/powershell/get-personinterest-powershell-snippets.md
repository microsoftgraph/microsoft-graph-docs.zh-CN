---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad2412d1479242eb72bac3bd849310b137450912
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350506"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileInterest -UserId $userId -PersonInterestId $personInterestId

```