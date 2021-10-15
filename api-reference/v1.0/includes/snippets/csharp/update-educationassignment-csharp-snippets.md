---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ad1d5116817d74155a31fc005e6f3be8deda21d
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60365802"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignment = new EducationAssignment
{
    DisplayName = "Reading and review test 09.03 #5",
    Instructions = new EducationItemBody
    {
        ContentType = BodyType.Text,
        Content = "Read chapter 5 and write your review"
    },
    DueDateTime = DateTimeOffset.Parse("2021-09-10T00:00:00Z"),
    AddedStudentAction = EducationAddedStudentAction.None
};

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"]
    .Request()
    .UpdateAsync(educationAssignment);

```