---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96b5b189ba4d86e616268c01c5ab1bfd4a60544b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351406"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileAnniversary -UserId $userId

```