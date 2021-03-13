---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 862d8c1220bbf6326ce65919f753d1bb6d18a4fc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797360"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationRubric = new EducationRubric
{
    DisplayName = "Example Credit Rubric after display name patch"
};

await graphClient.Education.Me.Rubrics["{educationRubric-id}"]
    .Request()
    .UpdateAsync(educationRubric);

```