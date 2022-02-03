---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a6fe0e8719ba19540373c9bc1c7388194fa974c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349541"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Remove-MgUserProfilePosition -UserId $userId -WorkPositionId $workPositionId

```