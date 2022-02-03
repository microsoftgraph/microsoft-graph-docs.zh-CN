---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a69afb1b9e8595468a5b32b77fca9c6601c92d20
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350162"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Remove-MgUserProfileAnniversary -UserId $userId -PersonAnnualEventId $personAnnualEventId

```