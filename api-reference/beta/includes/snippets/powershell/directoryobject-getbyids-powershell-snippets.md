---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2abf6ad49ef906429e091a5b0c01600bad3748aa
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346059"
---
```powershell

Import-Module Microsoft.Graph.DirectoryObjects

$params = @{
    Ids = @(
        "84b80893-8749-40a3-97b7-68513b600544"
        "5d6059b6-368d-45f8-91e1-8e07d485f1d0"
    )
    Types = @(
        "user"
    )
}

Get-MgDirectoryObjectById -BodyParameter $params

```