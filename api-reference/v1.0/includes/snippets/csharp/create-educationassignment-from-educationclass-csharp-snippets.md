---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f22c1feab6f8a577e69ebdc27d1f873f1b59cf8b
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60365844"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignment = new EducationAssignment
{
    DueDateTime = DateTimeOffset.Parse("2021-09-07T00:00:00Z"),
    DisplayName = "Reading test 09.03 #4",
    Instructions = new EducationItemBody
    {
        ContentType = BodyType.Text,
        Content = "Read chapter 4"
    },
    Grading = new EducationAssignmentPointsGradeType
    {
        MaxPoints = 50f
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