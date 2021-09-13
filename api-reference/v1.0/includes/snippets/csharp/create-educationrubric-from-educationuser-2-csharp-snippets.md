---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e484a54978306aa638b4c6f370d3ddfccc08bda0144fcdf0ad2c125ca326ef59
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278569"
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
            Grading = new EducationAssignmentPointsGradeType
            {
                MaxPoints = 2f
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
            Grading = new EducationAssignmentPointsGradeType
            {
                MaxPoints = 1f
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
            Weight = 50f
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
            Weight = 50f
        }
    },
    Grading = new EducationAssignmentPointsGradeType
    {
    }
};

await graphClient.Education.Me.Rubrics
    .Request()
    .AddAsync(educationRubric);

```