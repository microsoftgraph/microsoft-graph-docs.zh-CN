---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0af90e7bc838ea7808cd949ef151c4357f85f3d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351405"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Remove-MgUserProfile -UserId $userId

```