---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a72ec03bd748fa2d794123c376011d66d2071d5
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344051"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    MemberId = "319b41e8-d9e4-42f8-bdc9-741113f48b33"
}

Test-MgGroupDynamicMembership -GroupId $groupId -BodyParameter $params

```