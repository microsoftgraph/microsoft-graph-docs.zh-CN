---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b398b54b549a6a23cefdf7aa4e391d18e69b2f2
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992923"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationRubric = new EducationRubric
{
    DisplayName = "Example Credit Rubric",
    Description = new EducationItemBody
    {
        Content = "This is an example of a credit rubric (no points)",
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
            }
        },
        new RubricLevel
        {
            DisplayName = "Poor",
            Description = new EducationItemBody
            {
                Content = "",
                ContentType = BodyType.Text
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
            }
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
            }
        }
    }
};

await graphClient.Education.Me.Rubrics
    .Request()
    .AddAsync(educationRubric);

```