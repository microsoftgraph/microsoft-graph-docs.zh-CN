---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a18fc60d364d834eb5e449fe875d69c0c880b3cf
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60560397"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSubmissionResource = new EducationSubmissionResource
{
    Resource = new EducationExcelResource
    {
        DisplayName = "userAgeGroup QueryParameter Test.xlsx",
        FileUrl = "https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RONPUDM2CZKNRF3TGHYUM7Z64WE"
    }
};

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"].Resources
    .Request()
    .AddAsync(educationSubmissionResource);

```