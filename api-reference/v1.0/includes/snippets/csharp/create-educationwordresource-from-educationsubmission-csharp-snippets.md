---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 942f2abff97f6db34e1462d16ed0d862abb166c4
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60560396"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSubmissionResource = new EducationSubmissionResource
{
    Resource = new EducationWordResource
    {
        DisplayName = "Report.docx",
        FileUrl = "https://graph.microsoft.com/v1.0/drives/b!DPA6q59Tw0mtgmyXRUmrQRqBZTesG-lMkl1cBmvvMeUEWrOk89nKRpUEr4ZhNYBc/items/016XPCQEELISJB7NVNVBAK7V4UIF6Q27U2"
    }
};

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"].Resources
    .Request()
    .AddAsync(educationSubmissionResource);

```