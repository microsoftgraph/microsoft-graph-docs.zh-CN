---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f5088f384407a36a71fc20ed5d45924dd520538
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544173"
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
            Grading = new EducationAssignmentPointsGradeType
            {
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
    Grading = new EducationAssignmentPointsGradeType
    {
    }
};

await graphClient.Education.Me.Rubrics
    .Request()
    .AddAsync(educationRubric);

```