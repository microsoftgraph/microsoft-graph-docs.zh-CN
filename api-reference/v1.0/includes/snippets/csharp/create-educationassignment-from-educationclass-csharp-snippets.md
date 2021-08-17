---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a8b96340e2a56356637251f1060d984d27606fce7d282d8c1486cde0cf9b352
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221427"
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