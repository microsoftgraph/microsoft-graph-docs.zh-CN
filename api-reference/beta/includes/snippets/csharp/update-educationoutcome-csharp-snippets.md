---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64dd2b892369abbc94e17515c9671d371d5573c9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792507"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationOutcome = new EducationRubricOutcome
{
    RubricQualityFeedback = new List<RubricQualityFeedbackModel>()
    {
        new RubricQualityFeedbackModel
        {
            QualityId = "9a145aa8-f3d9-43a1-8f77-5387ff0693f2",
            Feedback = new EducationItemBody
            {
                Content = "This is feedback specific to the first quality of the rubric.",
                ContentType = BodyType.Text
            }
        },
        new RubricQualityFeedbackModel
        {
            QualityId = "d2331fb2-2761-402e-8de6-93e0afaa076e",
            Feedback = new EducationItemBody
            {
                Content = "This is feedback specific to the second quality of the rubric.",
                ContentType = BodyType.Text
            }
        }
    },
    RubricQualitySelectedLevels = new List<RubricQualitySelectedColumnModel>()
    {
        new RubricQualitySelectedColumnModel
        {
            QualityId = "9a145aa8-f3d9-43a1-8f77-5387ff0693f2",
            ColumnId = "4fb17a1d-5681-46c2-a295-4e305c3eae23"
        },
        new RubricQualitySelectedColumnModel
        {
            QualityId = "d2331fb2-2761-402e-8de6-93e0afaa076e",
            ColumnId = "aac076bf-51ba-48c5-a2e0-ee235b0b9740"
        }
    }
};

await graphClient.Education.Me.Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"].Outcomes["{educationOutcome-id}"]
    .Request()
    .UpdateAsync(educationOutcome);

```