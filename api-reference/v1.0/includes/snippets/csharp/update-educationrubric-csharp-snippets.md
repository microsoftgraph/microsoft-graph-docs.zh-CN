---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 862d8c1220bbf6326ce65919f753d1bb6d18a4fc
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52990959"
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