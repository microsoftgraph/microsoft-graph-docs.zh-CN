---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 908001069757d5262ebf6990cd7d9e45f98670e7
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350944"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileAnniversary -UserId $userId -PersonAnnualEventId $personAnnualEventId

```