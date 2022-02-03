---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15258cda67d3aec36c7ee113410d93b46657e91c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352168"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Remove-MgUserProfileWebAccount -UserId $userId -WebAccountId $webAccountId

```