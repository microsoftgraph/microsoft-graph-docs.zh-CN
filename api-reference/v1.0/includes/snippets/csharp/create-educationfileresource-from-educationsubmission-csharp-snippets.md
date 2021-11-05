---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87a0e5de7afd5d48102e0d7dbf9cc06bad72a33b
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60560398"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSubmissionResource = new EducationSubmissionResource
{
    Resource = new EducationFileResource
    {
        DisplayName = "_FTP_EDC-61424749-250820211136.pdf",
        FileUrl = "https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RL45XVPGDBRW5FLDR62Z5TCMGG3"
    }
};

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"].Resources
    .Request()
    .AddAsync(educationSubmissionResource);

```