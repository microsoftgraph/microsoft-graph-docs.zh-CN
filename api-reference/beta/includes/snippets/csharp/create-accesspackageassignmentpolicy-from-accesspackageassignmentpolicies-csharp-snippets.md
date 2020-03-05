---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c8f8ec89404c27df5ba2f3b854115db98716b62
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448443"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentPolicy = new AccessPackageAssignmentPolicy
{
    AccessPackageId = "56ff43fd-6b05-48df-9634-956a777fce6d",
    DisplayName = "direct",
    Description = "direct assignments by administrator",
    IsDenyPolicy = false,
    AccessReviewSettings = null,
    RequestorSettings = new RequestorSettings
    {
        ScopeType = "NoSubjects",
        AcceptRequests = true,
        AllowedRequestors = new List<UserSet>()
        {
        }
    },
    RequestApprovalSettings = new ApprovalSettings
    {
        IsApprovalRequired = false,
        IsApprovalRequiredForExtension = false,
        IsRequestorJustificationRequired = false,
        ApprovalMode = "NoApproval",
        ApprovalStages = new List<ApprovalStage>()
        {
        }
    }
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentPolicies
    .Request()
    .AddAsync(accessPackageAssignmentPolicy);

```