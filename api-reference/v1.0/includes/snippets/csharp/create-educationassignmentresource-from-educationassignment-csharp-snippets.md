---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c3c2708244153f4d303e585aedebc4fbd3b1f3d
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992791"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignmentResource = new EducationAssignmentResource
{
    DistributeForStudentWork = false,
    Resource = new EducationLinkResource
    {
        DisplayName = "Bing",
        Link = "https://www.bing.com"
    }
};

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Resources
    .Request()
    .AddAsync(educationAssignmentResource);

```