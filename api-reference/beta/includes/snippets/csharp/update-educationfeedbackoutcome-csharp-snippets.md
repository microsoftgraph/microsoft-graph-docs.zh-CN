---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e5a2a04d15c4b9e9cc22e8396420ac27c07e79b
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681701"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationOutcome = new EducationFeedbackOutcome
{
    Feedback = new EducationFeedback
    {
        Text = new EducationItemBody
        {
            Content = "This is feedback for the assignment as a whole.",
            ContentType = BodyType.Text
        }
    }
};

await graphClient.Education.Me.Assignments["{id}"].Submissions["{id}"].Outcomes["{id}"]
    .Request()
    .UpdateAsync(educationOutcome);

```