---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e827ed22a63b330b8046f40c6d03dde882189033
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209603"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentPolicy = new AccessPackageAssignmentPolicy
{
    DisplayName = "policy for external access requests",
    Description = "policy for users from connected organizations to request access, with two stages of approval.",
    AllowedTargetScope = AllowedTargetScope.AllConfiguredConnectedOrganizationUsers,
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
        EnableTargetsToSelfUpdateAccess = true,
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
                DurationBeforeAutomaticDenial = new Duration("P14D"),
                IsApproverJustificationRequired = false,
                IsEscalationEnabled = false,
                DurationBeforeEscalation = new Duration("PT0S"),
                PrimaryApprovers = new List<SubjectSet>()
                {
                    new InternalSponsors
                    {
                    }
                },
                FallbackPrimaryApprovers = new List<SubjectSet>()
                {
                    new SingleUser
                    {
                        UserId = "7deff43e-1f17-44ef-9e5f-d516b0ba11d4"
                    },
                    new GroupMembers
                    {
                        GroupId = "1623f912-5e86-41c2-af47-39dd67582b66"
                    }
                },
                EscalationApprovers = new List<SubjectSet>()
                {
                },
                FallbackEscalationApprovers = new List<SubjectSet>()
                {
                }
            },
            new AccessPackageApprovalStage
            {
                DurationBeforeAutomaticDenial = new Duration("P14D"),
                IsApproverJustificationRequired = false,
                IsEscalationEnabled = false,
                DurationBeforeEscalation = new Duration("PT0S"),
                PrimaryApprovers = new List<SubjectSet>()
                {
                },
                FallbackPrimaryApprovers = new List<SubjectSet>()
                {
                    new SingleUser
                    {
                        UserId = "46184453-e63b-4f20-86c2-c557ed5d5df9"
                    },
                    new GroupMembers
                    {
                        GroupId = "1623f912-5e86-41c2-af47-39dd67582b66"
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
        Id = "a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b"
    }
};

await graphClient.IdentityGovernance.EntitlementManagement.AssignmentPolicies
    .Request()
    .AddAsync(accessPackageAssignmentPolicy);

```