---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4470f58d67f34a51ea7d065245bfd17468300d1c
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436322"
---
```powershell

Import-Module Microsoft.Graph.Search

$params = @{
    Id = "e5477431-1038-484e-bf69-1dfedb97a110"
    Type = "externalGroup"
}

New-MgExternalConnectionGroupMember -ExternalConnectionId $externalConnectionId -ExternalGroupId $externalGroupId -BodyParameter $params

```