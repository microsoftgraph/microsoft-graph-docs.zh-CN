---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e2991eef869884487e53e0de86f2a73a4b8d52a
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442547"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    Displayname = "My legalHold with sources"
    Description = "Created from Graph API"
    ContentQuery = "Bazooka"
    "UserSources@odata.bind" = @(
        @{
            "@odata.type" = "microsoft.graph.security.userSource"
            Email = "SalesTeam@M365x809305.OnMicrosoft.com"
        }
    )
    "SiteSources@odata.bind" = @(
        @{
            "@odata.type" = "microsoft.graph.security.siteSource"
        }
    )
}

New-MgSecurityCaseEdiscoveryCaseLegalHold -EdiscoveryCaseId $ediscoveryCaseId -BodyParameter $params

```