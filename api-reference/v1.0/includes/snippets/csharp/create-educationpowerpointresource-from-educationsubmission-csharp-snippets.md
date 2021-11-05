---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 28419e1fc34cfa5664bbe7cc1995a2998255f3e8
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60560399"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSubmissionResource = new EducationSubmissionResource
{
    Resource = new EducationPowerPointResource
    {
        DisplayName = "state diagram.pptx",
        FileUrl = "https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RN3MHWWM7BNXJD2UD5OMRFEDKN2"
    }
};

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"].Resources
    .Request()
    .AddAsync(educationSubmissionResource);

```