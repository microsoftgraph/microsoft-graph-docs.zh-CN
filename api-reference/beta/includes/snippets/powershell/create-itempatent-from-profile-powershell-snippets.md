---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93e0ad71add097de4875ebec1b6b27496165d63f
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350294"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Description = "Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel."
    DisplayName = "Inferring User Intent through browsing behaviors"
    IsPending = $true
    Number = "USPTO-3954432633"
    WebUrl = "https://patents.gov/3954432633"
}

# A UPN can also be used as -UserId.
New-MgUserProfilePatent -UserId $userId -BodyParameter $params

```