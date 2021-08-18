---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a34d0aed9672635c346aef19b5355c2527943214
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368866"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentRequest = new AccessPackageAssignmentRequestObject
{
    RequestType = "UserAdd",
    AccessPackageAssignment = new AccessPackageAssignment
    {
        TargetId = "46184453-e63b-4f20-86c2-c557ed5d5df9",
        AssignmentPolicyId = "2264bf65-76ba-417b-a27d-54d291f0cbc8",
        AccessPackageId = "a914b616-e04e-476b-aa37-91038f0b165b"
    },
    Answers = new List<AccessPackageAnswer>()
    {
        new AccessPackageAnswerString
        {
            Value = "Arizona",
            AnsweredQuestion = new AccessPackageMultipleChoiceQuestion
            {
                Id = "A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF"
            }
        },
        new AccessPackageAnswerString
        {
            Value = "Need access to marketing campaign material",
            AnsweredQuestion = new AccessPackageTextInputQuestion
            {
                Id = "AA615EE9-D9D8-4C03-BE91-BEE37106DEDA"
            }
        }
    }
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentRequests
    .Request()
    .AddAsync(accessPackageAssignmentRequest);

```