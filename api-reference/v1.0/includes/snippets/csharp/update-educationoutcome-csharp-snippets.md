---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bcbaec37d80324fd5cad35feb15f93ee525d15ed
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991298"
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

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"].Outcomes["{educationOutcome-id}"]
    .Request()
    .UpdateAsync(educationOutcome);

```