---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 07cf54822bd266657d8526f7c20e0c27c33c176c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461234"
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