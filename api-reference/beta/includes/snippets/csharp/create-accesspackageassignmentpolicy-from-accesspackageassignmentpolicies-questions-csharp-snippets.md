---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25429d4a90b27d37b0852908a834d87ed03c789a685182605c3863f242d1f9a7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902806"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentPolicy = new AccessPackageAssignmentPolicy
{
    AccessPackageId = "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
    DisplayName = "Users from connected organizations can request",
    Description = "Allow users from configured connected organizations to request and be approved by their sponsors",
    CanExtend = false,
    DurationInDays = 365,
    ExpirationDateTime = null,
    RequestorSettings = new RequestorSettings
    {
        ScopeType = "AllExistingConnectedOrganizationSubjects",
        AcceptRequests = true
    },
    RequestApprovalSettings = new ApprovalSettings
    {
        IsApprovalRequired = true,
        IsApprovalRequiredForExtension = false,
        IsRequestorJustificationRequired = true,
        ApprovalMode = "SingleStage",
        ApprovalStages = new List<ApprovalStage>()
        {
            new ApprovalStage
            {
                ApprovalStageTimeOutInDays = 14,
                IsApproverJustificationRequired = true,
                IsEscalationEnabled = false,
                EscalationTimeInMinutes = 11520,
                PrimaryApprovers = new List<UserSet>()
                {
                    new GroupMembers
                    {
                        IsBackup = true,
                        Id = "d2dcb9a1-a445-42ee-83a8-476522ed6cbf",
                        Description = "group for users from connected organizations which have no external sponsor"
                    },
                    new ExternalSponsors
                    {
                        IsBackup = false
                    }
                }
            }
        }
    },
    Questions = new List<AccessPackageQuestion>()
    {
        new AccessPackageMultipleChoiceQuestion
        {
            IsRequired = false,
            Text = new AccessPackageLocalizedContent
            {
                DefaultText = "what state are you from?",
                LocalizedTexts = new List<AccessPackageLocalizedText>()
                {
                    new AccessPackageLocalizedText
                    {
                        Text = "¿De qué estado eres?",
                        LanguageCode = "es"
                    }
                }
            },
            Choices = new List<AccessPackageAnswerChoice>()
            {
                new AccessPackageAnswerChoice
                {
                    ActualValue = "AZ",
                    DisplayValue = new AccessPackageLocalizedContent
                    {
                        LocalizedTexts = new List<AccessPackageLocalizedText>()
                        {
                            new AccessPackageLocalizedText
                            {
                                Text = "Arizona",
                                LanguageCode = "es"
                            }
                        }
                    }
                },
                new AccessPackageAnswerChoice
                {
                    ActualValue = "CA",
                    DisplayValue = new AccessPackageLocalizedContent
                    {
                        LocalizedTexts = new List<AccessPackageLocalizedText>()
                        {
                            new AccessPackageLocalizedText
                            {
                                Text = "California",
                                LanguageCode = "es"
                            }
                        }
                    }
                },
                new AccessPackageAnswerChoice
                {
                    ActualValue = "OH",
                    DisplayValue = new AccessPackageLocalizedContent
                    {
                        LocalizedTexts = new List<AccessPackageLocalizedText>()
                        {
                            new AccessPackageLocalizedText
                            {
                                Text = "Ohio",
                                LanguageCode = "es"
                            }
                        }
                    }
                }
            },
            AllowsMultipleSelection = false
        },
        new AccessPackageTextInputQuestion
        {
            IsRequired = false,
            Text = new AccessPackageLocalizedContent
            {
                DefaultText = "Who is your manager?",
                LocalizedTexts = new List<AccessPackageLocalizedText>()
                {
                    new AccessPackageLocalizedText
                    {
                        Text = "por qué necesita acceso a este paquete",
                        LanguageCode = "es"
                    }
                }
            },
            IsSingleLineQuestion = false
        }
    }
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentPolicies
    .Request()
    .AddAsync(accessPackageAssignmentPolicy);

```