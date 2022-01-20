---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42d24a105ae18dc13ed5f5fb41a700f3d9fe44b3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120500"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    AccessPackageId = "b2eba9a1-b357-42ee-83a8-336522ed6cbf"
    DisplayName = "Users from connected organizations can request"
    Description = "Allow users from configured connected organizations to request and be approved by their sponsors"
    CanExtend = $false
    DurationInDays = 365
    ExpirationDateTime = $null
    RequestorSettings = @{
        ScopeType = "AllExistingConnectedOrganizationSubjects"
        AcceptRequests = $true
    }
    RequestApprovalSettings = @{
        IsApprovalRequired = $true
        IsApprovalRequiredForExtension = $false
        IsRequestorJustificationRequired = $true
        ApprovalMode = "SingleStage"
        ApprovalStages = @(
            @{
                ApprovalStageTimeOutInDays = 14
                IsApproverJustificationRequired = $true
                IsEscalationEnabled = $false
                EscalationTimeInMinutes = 11520
                PrimaryApprovers = @(
                    @{
                        "@odata.type" = "#microsoft.graph.groupMembers"
                        IsBackup = $true
                        Id = "d2dcb9a1-a445-42ee-83a8-476522ed6cbf"
                        Description = "group for users from connected organizations which have no external sponsor"
                    }
                    @{
                        "@odata.type" = "#microsoft.graph.externalSponsors"
                        IsBackup = $false
                    }
                )
            }
        )
    }
    Questions = @(
        @{
            IsRequired = $false
            Text = @{
                DefaultText = "what state are you from?"
                LocalizedTexts = @(
                    @{
                        Text = "¿De qué estado eres?"
                        LanguageCode = "es"
                    }
                )
            }
            "@odata.type" = "#microsoft.graph.accessPackageMultipleChoiceQuestion"
            Choices = @(
            )
            AllowsMultipleSelection = $false
        }
        @{
            IsRequired = $false
            Text = @{
                DefaultText = "Who is your manager?"
                LocalizedTexts = @(
                    @{
                        Text = "por qué necesita acceso a este paquete"
                        LanguageCode = "es"
                    }
                )
            }
            "@odata.type" = "#microsoft.graph.accessPackageTextInputQuestion"
            IsSingleLineQuestion = $false
        }
    )
}

New-MgEntitlementManagementAccessPackageAssignmentPolicy -BodyParameter $params

```