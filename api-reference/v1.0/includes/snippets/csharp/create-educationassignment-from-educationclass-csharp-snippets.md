---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e8d25b20486c864beb24c35829b45d4550d5114
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992119"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignment = new EducationAssignment
{
    DueDateTime = DateTimeOffset.Parse("2014-02-01T00:00:00Z"),
    DisplayName = "Midterm 1",
    Instructions = new EducationItemBody
    {
        ContentType = BodyType.Text,
        Content = "Read chapters 1 through 3"
    },
    Grading = new EducationAssignmentPointsGradeType
    {
        MaxPoints = 100f
    },
    AssignTo = new EducationAssignmentClassRecipient
    {
    },
    Status = EducationAssignmentStatus.Draft,
    AllowStudentsToAddResourcesToSubmission = true
};

await graphClient.Education.Classes["{educationClass-id}"].Assignments
    .Request()
    .AddAsync(educationAssignment);

```