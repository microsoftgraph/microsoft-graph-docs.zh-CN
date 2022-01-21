---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 73d9d4d32d4dd446fd39d5bf66fe788643f7431a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62119474"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    DisplayName = "Seattle District Technical Schools"
    Description = "Seattle district technical schools administration"
    Visibility = "HiddenMembership"
}

New-MgAdministrativeUnit -BodyParameter $params

```