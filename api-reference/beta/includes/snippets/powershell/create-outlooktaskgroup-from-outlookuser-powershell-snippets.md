---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68cebb9d552e6ec51ee3209f1a1c73c3891aa126
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089613"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    Name = "Leisure tasks"
}

New-MgUserOutlookTaskGroup -UserId $userId -BodyParameter $params

```