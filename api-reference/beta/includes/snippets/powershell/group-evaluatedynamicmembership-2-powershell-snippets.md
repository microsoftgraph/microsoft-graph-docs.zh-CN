---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b921d0e09f3869b08fc5b442b4f6b30facab450
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819489"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    MemberId = "319b41e8-d9e4-42f8-bdc9-741113f48b33"
    MembershipRule = "(user.displayName -startsWith "EndTestUser")"
}

Test-MgGroupDynamicMembershipRule -BodyParameter $params

```