---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84d5937913916ae4428a0dbec728dc0407a752ba
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681704"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationOutcome = new EducationPointsOutcome
{
    Points = new EducationAssignmentPointsGrade
    {
        Points = 85f
    }
};

await graphClient.Education.Me.Assignments["{id}"].Submissions["{id}"].Outcomes["{id}"]
    .Request()
    .UpdateAsync(educationOutcome);

```