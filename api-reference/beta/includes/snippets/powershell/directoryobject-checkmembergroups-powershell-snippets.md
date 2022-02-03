---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9052076085008f9280357e056e0958f2b267ef97
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62345642"
---
```powershell

Import-Module Microsoft.Graph.DirectoryObjects

$params = @{
    GroupIds = @(
        "f448435d-3ca7-4073-8152-a1fd73c0fd09"
        "bd7c6263-4dd5-4ae8-8c96-556e1c0bece6"
        "93670da6-d731-4366-94b5-abed40b6016b"
        "f5484ab1-4d4d-41ec-a9b8-754b3957bfc7"
        "c9103f26-f3cf-4004-a611-2a14e81b8f79"
    )
}

Confirm-MgDirectoryObjectMemberGroup -DirectoryObjectId $directoryObjectId -BodyParameter $params

```