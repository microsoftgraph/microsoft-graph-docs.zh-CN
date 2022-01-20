---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4cf989e83297a91407717d1f324c0eeb3f49921
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125018"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    DisplayName = "Seattle District Technical Schools"
    Description = "Seattle district technical schools administration"
    Visibility = "HiddenMembership"
}

New-MgDirectoryAdministrativeUnit -BodyParameter $params

```