---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21f3aaeeda2115fa1f0f0ae27a53508fe6cf98bd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101006"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    DisplayName = "Example Credit Rubric"
    Description = @{
        Content = "This is an example of a credit rubric (no points)"
        ContentType = "text"
    }
    Levels = @(
        @{
            DisplayName = "Good"
            Description = @{
                Content = ""
                ContentType = "text"
            }
        }
        @{
            DisplayName = "Poor"
            Description = @{
                Content = ""
                ContentType = "text"
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
        }
    )
}

New-MgEducationMeRubric -BodyParameter $params

```