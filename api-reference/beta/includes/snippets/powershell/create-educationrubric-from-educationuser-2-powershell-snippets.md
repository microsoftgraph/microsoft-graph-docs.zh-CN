---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89b533b6c972ccfc8fb76c17859db9207a6f8f94
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62096491"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    DisplayName = "Example Points Rubric"
    Description = @{
        Content = "This is an example of a rubric with points"
        ContentType = "text"
    }
    Levels = @(
        @{
            DisplayName = "Good"
            Description = @{
                Content = ""
                ContentType = "text"
            }
            Grading = @{
                "@odata.type" = "#microsoft.graph.educationAssignmentPointsGradeType"
                MaxPoints = 
            }
        }
        @{
            DisplayName = "Poor"
            Description = @{
                Content = ""
                ContentType = "text"
            }
            Grading = @{
                "@odata.type" = "#microsoft.graph.educationAssignmentPointsGradeType"
                MaxPoints = 
            }
        }
    )
    Qualities = @(
        @{
            Description = @{
                Content = "Argument"
                ContentType = "text"
            }
            Criteria = @(
                @{
                    Description = @{
                        Content = "The essay's argument is persuasive."
                        ContentType = "text"
                    }
                }
                @{
                    Description = @{
                        Content = "The essay's argument does not make sense."
                        ContentType = "text"
                    }
                }
            )
            Weight = 50.0
        }
        @{
            Description = @{
                Content = "Spelling and Grammar"
                ContentType = "text"
            }
            Criteria = @(
                @{
                    Description = @{
                        Content = "The essay uses proper spelling and grammar with few or no errors."
                        ContentType = "text"
                    }
                }
                @{
                    Description = @{
                        Content = "The essay has numerous errors in spelling and/or grammar."
                        ContentType = "text"
                    }
                }
            )
            Weight = 50.0
        }
    )
    Grading = @{
        "@odata.type" = "#microsoft.graph.educationAssignmentPointsGradeType"
    }
}

New-MgEducationMeRubric -BodyParameter $params

```