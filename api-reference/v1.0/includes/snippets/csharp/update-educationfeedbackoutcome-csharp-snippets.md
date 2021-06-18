---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4bd4a3009984b44ede3ea02ce300334f8f08cfa
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991295"
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