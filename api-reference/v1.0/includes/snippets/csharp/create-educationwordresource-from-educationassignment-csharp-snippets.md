---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68fddde0247672ccdd38b2f6d46864f2f18bfb46
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60558726"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignmentResource = new EducationAssignmentResource
{
    DistributeForStudentWork = false,
    Resource = new EducationWordResource
    {
        DisplayName = "Issues and PR in guthub.docx",
        FileUrl = "https://graph.microsoft.com/v1.0/drives/b!DPA6q59Tw0mtgmyXRUmrQRqBZTesG-lMkl1cBmvvMeUEWrOk89nKRpUEr4ZhNYBc/items/016XPCQEELISJB7NVNVBAK7V4UIF6Q27U2"
    }
};

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Resources
    .Request()
    .AddAsync(educationAssignmentResource);

```