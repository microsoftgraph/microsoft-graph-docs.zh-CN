---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a075d35c0b2198d3086a7672477eca9d8c40385
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120498"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    AccessPackageId = "string (identifier)"
    DisplayName = "Users from connected organizations can request"
    Description = "Allow users from configured connected organizations to request and be approved by their sponsors"
    CanExtend = $false
    DurationInDays = 365
    ExpirationDateTime = $null
    RequestorSettings = @{
        ScopeType = "AllExistingConnectedOrganizationSubjects"
        AcceptRequests = $true
        AllowedRequestors = @(
        )
    }
    RequestApprovalSettings = @{
        IsApprovalRequired = $true
        IsApprovalRequiredForExtension = $false
        IsRequestorJustificationRequired = $true
        ApprovalMode = "Serial"
        ApprovalStages = @(
            @{
                ApprovalStageTimeOutInDays = 14
                IsApproverJustificationRequired = $true
                IsEscalationEnabled = $true
                EscalationTimeInMinutes = 11520
                PrimaryApprovers = @(
                    @{
                        "@odata.type" = "#microsoft.graph.groupMembers"
                        IsBackup = $true
                        Id = "string (identifier)"
                        Description = "group for users from connected organizations which have no external sponsor"
                    }
                    @{
                        "@odata.type" = "#microsoft.graph.externalSponsors"
                        IsBackup = $false
                    }
                )
                EscalationApprovers = @(
                    @{
                        "@odata.type" = "#microsoft.graph.singleUser"
                        IsBackup = $true
                        Id = "string (identifier)"
                        Description = "user if the external sponsor does not respond"
                    }
                )
            }
            @{
                ApprovalStageTimeOutInDays = 14
                IsApproverJustificationRequired = $true
                IsEscalationEnabled = $true
                EscalationTimeInMinutes = 11520
                PrimaryApprovers = @(
                    @{
                        "@odata.type" = "#microsoft.graph.groupMembers"
                        IsBackup = $true
                        Id = "string (identifier)"
                        Description = "group for users from connected organizations which have no internal sponsor"
                    }
                    @{
                        "@odata.type" = "#microsoft.graph.internalSponsors"
                        IsBackup = $false
                    }
                )
                EscalationApprovers = @(
                    @{
                        "@odata.type" = "#microsoft.graph.singleUser"
                        IsBackup = $true
                        Id = "string (identifier)"
                        Description = "user if the internal sponsor does not respond"
                    }
                )
            }
        )
    }
    AccessReviewSettings = @{
        IsEnabled = $true
        RecurrenceType = "quarterly"
        ReviewerType = "Self"
        StartDateTime = [System.DateTime]::Parse("2020-04-01T07:59:59.998Z")
        DurationInDays = 25
        Reviewers = @(
        )
    }
}

New-MgEntitlementManagementAccessPackageAssignmentPolicy -BodyParameter $params

```