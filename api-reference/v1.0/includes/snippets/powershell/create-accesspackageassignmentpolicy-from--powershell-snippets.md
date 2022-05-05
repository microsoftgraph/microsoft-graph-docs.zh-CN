---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ae1482d7387c93a37217791ed5e236250e03425
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209634"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    DisplayName = "New Policy"
    Description = "policy for assignment"
    AllowedTargetScope = "notSpecified"
    SpecificAllowedTargets = @(
    )
    Expiration = @{
        EndDateTime = $null
        Duration = $null
        Type = "noExpiration"
    }
    RequestorSettings = @{
        EnableTargetsToSelfAddAccess = $false
        EnableTargetsToSelfUpdateAccess = $false
        EnableTargetsToSelfRemoveAccess = $false
        AllowCustomAssignmentSchedule = $true
        EnableOnBehalfRequestorsToAddAccess = $false
        EnableOnBehalfRequestorsToUpdateAccess = $false
        EnableOnBehalfRequestorsToRemoveAccess = $false
        OnBehalfRequestors = @(
        )
    }
    RequestApprovalSettings = @{
        IsApprovalRequiredForAdd = $false
        IsApprovalRequiredForUpdate = $false
        Stages = @(
        )
    }
    AccessPackage = @{
        Id = "a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b"
    }
}

New-MgEntitlementManagementAssignmentPolicy -BodyParameter $params

```