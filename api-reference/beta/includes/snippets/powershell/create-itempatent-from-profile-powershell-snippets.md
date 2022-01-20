---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abf6f2398b8f2b4ac96c0d8c9e0a3c7b718c6331
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135217"
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

New-MgUserProfilePatent -UserId $userId -BodyParameter $params

```