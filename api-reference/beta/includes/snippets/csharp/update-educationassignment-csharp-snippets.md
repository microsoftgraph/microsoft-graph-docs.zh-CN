---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 21e0d8cb6934fc22059f3d0011636afaae2b62c3
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36845920"
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
    DueDateTime = DateTimeOffset.Parse("2014-02-01T00:00:00Z")
};

await graphClient.Education.Classes["11021"].Assignments["19002"]
    .Request()
    .UpdateAsync(educationAssignment);

```