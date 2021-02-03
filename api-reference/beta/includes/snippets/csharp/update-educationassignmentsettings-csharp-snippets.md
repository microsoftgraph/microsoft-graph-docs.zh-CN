---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b5053c417bb3047417ac4f5af2846e5ae81eec5
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092495"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignmentSettings = new EducationAssignmentSettings
{
    SubmissionAnimationDisabled = true
};

await graphClient.Education.Classes["{id}"].AssignmentSettings
    .Request()
    .UpdateAsync(educationAssignmentSettings);

```