---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 836bcb4197ed3eed4f3a8235e656a6b3ede0b21a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351269"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Remove-MgUserProfileEducationalActivity -UserId $userId -EducationalActivityId $educationalActivityId

```