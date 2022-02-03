---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6665b4457d341f6242e414e15c394f70d27b341b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342287"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Get-MgUser -UserId $userId

```