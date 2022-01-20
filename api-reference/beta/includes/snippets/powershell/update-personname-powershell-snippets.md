---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a48f86b57d2f1d4a48f25924e6117dfc40d6d45
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112389"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Nickname = "Kesha"
}

Update-MgUserProfileName -UserId $userId -PersonNameId $personNameId -BodyParameter $params

```