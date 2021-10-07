---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c1e36d374c7fb423da3777b7a5dccc95190b54e1bf096801b3ac5cd3adff173
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161560"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignment = new EducationAssignment
{
    DisplayName = "Week 1 reading assignment",
    Instructions = new EducationItemBody
    {
        ContentType = BodyType.Text,
        Content = "Read chapters 1 through 3"
    },
    DueDateTime = DateTimeOffset.Parse("2014-02-01T00:00:00Z"),
    AddedStudentAction = EducationAddedStudentAction.None,
    AddToCalendarAction = EducationAddToCalendarOptions.StudentsAndPublisher
};

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"]
    .Request()
    .UpdateAsync(educationAssignment);

```