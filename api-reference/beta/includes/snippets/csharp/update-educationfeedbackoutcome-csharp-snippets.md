---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07283254b282b2dbd2656c44f7a7e89cf80aeb9aaf65051e198629973a0ce04e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218561"
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

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"].Outcomes["{educationOutcome-id}"]
    .Request()
    .UpdateAsync(educationOutcome);

```