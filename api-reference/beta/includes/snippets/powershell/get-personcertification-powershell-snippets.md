---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a26fe759457418415b73d4e0ad5a1034d848b4b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352478"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileCertification -UserId $userId -PersonCertificationId $personCertificationId

```