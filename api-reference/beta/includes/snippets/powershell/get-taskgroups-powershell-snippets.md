---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af077febe3f13f601f0aeeac6e8a0e6ed078dff8
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352243"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Get-MgUserOutlookTaskGroup -UserId $userId

```