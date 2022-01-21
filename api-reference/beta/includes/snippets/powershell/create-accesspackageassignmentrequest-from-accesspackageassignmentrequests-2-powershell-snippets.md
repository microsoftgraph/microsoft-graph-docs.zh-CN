---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e6206340111fbf902f3747221a0ce6f0564abb0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129849"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    RequestType = "UserAdd"
    AccessPackageAssignment = @{
        TargetId = "46184453-e63b-4f20-86c2-c557ed5d5df9"
        AssignmentPolicyId = "2264bf65-76ba-417b-a27d-54d291f0cbc8"
        AccessPackageId = "a914b616-e04e-476b-aa37-91038f0b165b"
    }
    Answers = @(
        @{
            "@odata.type" = "#microsoft.graph.accessPackageAnswerString"
            Value = "Arizona"
            AnsweredQuestion = @{
                "@odata.type" = "#microsoft.graph.accessPackageMultipleChoiceQuestion"
                Id = "A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF"
            }
        }
        @{
            "@odata.type" = "#microsoft.graph.accessPackageAnswerString"
            Value = "Need access to marketing campaign material"
            AnsweredQuestion = @{
                "@odata.type" = "#microsoft.graph.accessPackageTextInputQuestion"
                Id = "AA615EE9-D9D8-4C03-BE91-BEE37106DEDA"
            }
        }
    )
}

New-MgEntitlementManagementAccessPackageAssignmentRequest -BodyParameter $params

```