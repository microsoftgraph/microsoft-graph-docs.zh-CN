---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1199f26785bf884601ffcbe93aa46d6776b3344bb76d9dba0421f2f09ad0a2f6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158652"
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