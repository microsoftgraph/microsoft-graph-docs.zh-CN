---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c78bf7988085d402c8eee56987c111688fe1cf50
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120499"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    AccessPackageId = "56ff43fd-6b05-48df-9634-956a777fce6d"
    DisplayName = "direct"
    Description = "direct assignments by administrator"
    AccessReviewSettings = $null
    RequestorSettings = @{
        ScopeType = "NoSubjects"
        AcceptRequests = $true
        AllowedRequestors = @(
        )
    }
    RequestApprovalSettings = @{
        IsApprovalRequired = $false
        IsApprovalRequiredForExtension = $false
        IsRequestorJustificationRequired = $false
        ApprovalMode = "NoApproval"
        ApprovalStages = @(
        )
    }
}

New-MgEntitlementManagementAccessPackageAssignmentPolicy -BodyParameter $params

```