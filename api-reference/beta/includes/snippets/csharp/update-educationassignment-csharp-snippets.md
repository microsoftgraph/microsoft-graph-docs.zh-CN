---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 07cf54822bd266657d8526f7c20e0c27c33c176c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712871"
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
    DueDateTime = "2014-02-01T00:00:00Z"
};

await graphClient.Education.Classes["11021"].Assignments["19002"]
    .Request()
    .UpdateAsync(educationAssignment);

```