---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 412d8a7d45225a779a666364deaaaa3aa5170f51
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992339"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationCategory = new EducationCategory
{
    DisplayName = "Quizzes"
};

await graphClient.Education.Classes["{educationClass-id}"].AssignmentCategories
    .Request()
    .AddAsync(educationCategory);

```