---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39258904e69bedac9fe471d64334cba8379054f6
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339543"
---
```powershell

Import-Module Microsoft.Graph.DirectoryObjects

$params = @{
    Ids = @(
        "84b80893874940a3-97b7-68513b600544"
        "5d6059b6368d-45f8-91e18e07d485f1d0"
    )
    Types = @(
        "user"
    )
}

Get-MgDirectoryObjectById -BodyParameter $params

```