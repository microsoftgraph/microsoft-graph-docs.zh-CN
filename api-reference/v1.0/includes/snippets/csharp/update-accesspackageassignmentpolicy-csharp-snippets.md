---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0e161e4053317534502d7f1f0ba62d16c923942
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209862"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentPolicy = new AccessPackageAssignmentPolicy
{
    Id = "87e1c7f7-c7f7-87e1-f7c7-e187f7c7e187",
    DisplayName = "All Users",
    Description = "All users can request for access to the directory.",
    AllowedTargetScope = AllowedTargetScope.AllDirectoryUsers,
    SpecificAllowedTargets = new List<SubjectSet>()
    {
    },
    Expiration = new ExpirationPattern
    {
        Type = ExpirationPatternType.NoExpiration
    },
    RequestorSettings = new AccessPackageAssignmentRequestorSettings
    {
        EnableTargetsToSelfAddAccess = true,
        EnableTargetsToSelfUpdateAccess = false,
        EnableTargetsToSelfRemoveAccess = true,
        AllowCustomAssignmentSchedule = false,
        EnableOnBehalfRequestorsToAddAccess = false,
        EnableOnBehalfRequestorsToUpdateAccess = false,
        EnableOnBehalfRequestorsToRemoveAccess = false,
        OnBehalfRequestors = new List<SubjectSet>()
        {
        }
    },
    RequestApprovalSettings = new AccessPackageAssignmentApprovalSettings
    {
        IsApprovalRequiredForAdd = true,
        IsApprovalRequiredForUpdate = false,
        Stages = new List<AccessPackageApprovalStage>()
        {
            new AccessPackageApprovalStage
            {
                DurationBeforeAutomaticDenial = new Duration("P2D"),
                IsApproverJustificationRequired = false,
                IsEscalationEnabled = false,
                DurationBeforeEscalation = new Duration("PT0S"),
                PrimaryApprovers = new List<SubjectSet>()
                {
                    new RequestorManager
                    {
                        ManagerLevel = 1
                    }
                },
                FallbackPrimaryApprovers = new List<SubjectSet>()
                {
                    new SingleUser
                    {
                        UserId = "e6bf4d7d-6824-4dd0-809d-5bf42d4817c2",
                        Description = "user"
                    }
                },
                EscalationApprovers = new List<SubjectSet>()
                {
                },
                FallbackEscalationApprovers = new List<SubjectSet>()
                {
                }
            }
        }
    },
    AccessPackage = new AccessPackage
    {
        Id = "49d2c59b-0a81-463d-a8ec-ddad3935d8a0"
    }
};

await graphClient.IdentityGovernance.EntitlementManagement.AssignmentPolicies["{accessPackageAssignmentPolicy-id}"]
    .Request()
    .PutAsync(accessPackageAssignmentPolicy);

```