---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0ec1a901602e364864c14d433393d722eb88405
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442276"
---
```powershell

Import-Module Microsoft.Graph.Search

$params = @{
    Id = "1431b9c38ee647f6a"
    Type = "externalGroup"
}

New-MgExternalConnectionGroupMember -ExternalConnectionId $externalConnectionId -ExternalGroupId $externalGroupId -BodyParameter $params

```