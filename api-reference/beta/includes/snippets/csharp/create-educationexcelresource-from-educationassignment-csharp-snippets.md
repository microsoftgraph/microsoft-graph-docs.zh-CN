---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b9ea6305136e2f59dd97706e367cd97fc4a2ab6
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60559442"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignmentResource = new EducationAssignmentResource
{
    DistributeForStudentWork = false,
    Resource = new EducationExcelResource
    {
        DisplayName = "Graph Doc pages.xlsx",
        FileUrl = "https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RIR7PSV4JJSFJHKNPUVUWGPW4O2"
    }
};

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Resources
    .Request()
    .AddAsync(educationAssignmentResource);

```