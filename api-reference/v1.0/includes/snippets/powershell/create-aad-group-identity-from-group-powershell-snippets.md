---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 582ff52df265c3677a39f3b8c227d031e7b7a291
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442277"
---
```powershell

Import-Module Microsoft.Graph.Search

$params = @{
    Id = "e5477431-1038-484e-bf69-1dfedb97a110"
    Type = "group"
}

New-MgExternalConnectionGroupMember -ExternalConnectionId $externalConnectionId -ExternalGroupId $externalGroupId -BodyParameter $params

```