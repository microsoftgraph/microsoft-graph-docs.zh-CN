---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6fc50154c3e4983f2022ed4fbc74b30f35a1446
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871459"
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