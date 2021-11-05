---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4dd8a8a8de263875c901adc2f630b6e84dddce09
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60560400"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSubmissionResource = new EducationSubmissionResource
{
    Resource = new EducationLinkResource
    {
        DisplayName = "Wikipedia",
        Link = "https://en.wikipedia.org/wiki/Main_Page"
    }
};

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"].Resources
    .Request()
    .AddAsync(educationSubmissionResource);

```