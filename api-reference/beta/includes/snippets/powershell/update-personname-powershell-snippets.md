---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1359fe2b44cdc958e845f792c960dca33ff729f6
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349501"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Nickname = "Kesha"
}

# A UPN can also be used as -UserId.
Update-MgUserProfileName -UserId $userId -PersonNameId $personNameId -BodyParameter $params

```