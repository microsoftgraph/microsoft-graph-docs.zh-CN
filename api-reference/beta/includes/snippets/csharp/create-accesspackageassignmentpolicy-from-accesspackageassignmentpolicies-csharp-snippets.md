---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4085e99670bdd2b1c2d4f030083a066ad22c74e0
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589729"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentPolicy = new AccessPackageAssignmentPolicy
{
    AccessPackageId = "56ff43fd-6b05-48df-9634-956a777fce6d",
    DisplayName = "direct",
    Description = "direct assignments by administrator",
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