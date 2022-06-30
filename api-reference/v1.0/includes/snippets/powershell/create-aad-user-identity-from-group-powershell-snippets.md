---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba29b49d24322b261f0c4eb9d814ad4513245ded
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442278"
---
```powershell

Import-Module Microsoft.Graph.Search

$params = @{
    Id = "e811976d-83df-4cbd-8b9b-5215b18aa874"
    Type = "user"
}

New-MgExternalConnectionGroupMember -ExternalConnectionId $externalConnectionId -ExternalGroupId $externalGroupId -BodyParameter $params

```