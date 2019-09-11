---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 83394ed36bd0789dad614898854ce7d17c41ccd8
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36845921"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationRubric = new EducationRubric
{
    DisplayName = "Example Points Rubric",
    Description = new EducationItemBody
    {
        Content = "This is an example of a rubric with points",
        ContentType = BodyType.Text
    },
    Levels = new List<RubricLevel>()
    {
        new RubricLevel
        {
            DisplayName = "Good",
            Description = new EducationItemBody
            {
                Content = "",
                ContentType = BodyType.Text
            },
            Grading = new EducationAssignmentGradeType
            {
                AdditionalData = new Dictionary<string, object>()
                {
                    {"@odata.type","#microsoft.graph.educationAssignmentPointsGradeType"}
                },
                MaxPoints = 2
            }
        },
        new RubricLevel
        {
            DisplayName = "Poor",
            Description = new EducationItemBody
            {
                Content = "",
                ContentType = BodyType.Text
            },
            Grading = new EducationAssignmentGradeType
            {
                AdditionalData = new Dictionary<string, object>()
                {
                    {"@odata.type","#microsoft.graph.educationAssignmentPointsGradeType"}
                },
                MaxPoints = 1
            }
        }
    },
    Qualities = new List<RubricQuality>()
    {
        new RubricQuality
        {
            Description = new EducationItemBody
            {
                Content = "Argument",
                ContentType = BodyType.Text
            },
            Criteria = new List<RubricCriterion>()
            {
                new RubricCriterion
                {
                    Description = new EducationItemBody
                    {
                        Content = "The essay's argument is persuasive.",
                        ContentType = BodyType.Text
                    }
                },
                new RubricCriterion
                {
                    Description = new EducationItemBody
                    {
                        Content = "The essay's argument does not make sense.",
                        ContentType = BodyType.Text
                    }
                }
            },
            Weight = 50
        },
        new RubricQuality
        {
            Description = new EducationItemBody
            {
                Content = "Spelling and Grammar",
                ContentType = BodyType.Text
            },
            Criteria = new List<RubricCriterion>()
            {
                new RubricCriterion
                {
                    Description = new EducationItemBody
                    {
                        Content = "The essay uses proper spelling and grammar with few or no errors.",
                        ContentType = BodyType.Text
                    }
                },
                new RubricCriterion
                {
                    Description = new EducationItemBody
                    {
                        Content = "The essay has numerous errors in spelling and/or grammar.",
                        ContentType = BodyType.Text
                    }
                }
            },
            Weight = 50
        }
    },
    Grading = new EducationAssignmentGradeType
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"@odata.type","#microsoft.graph.educationAssignmentPointsGradeType"}
        }
    }
};

await graphClient.Education.Me.Rubrics
    .Request()
    .AddAsync(educationRubric);

```