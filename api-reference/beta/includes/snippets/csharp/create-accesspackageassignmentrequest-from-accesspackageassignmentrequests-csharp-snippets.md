---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 622fe1863c9ced1455a01bc4facc9d47b9bbbf91
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756095"
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
            AnsweredQuestion = new AccessPackageQuestion
            {
                Id = "A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF"
            }
        },
        new AccessPackageAnswerString
        {
            Value = "Need access to marketing campaign material",
            AnsweredQuestion = new AccessPackageQuestion
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