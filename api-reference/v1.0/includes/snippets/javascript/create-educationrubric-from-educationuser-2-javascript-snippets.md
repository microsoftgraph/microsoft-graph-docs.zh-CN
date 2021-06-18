---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 309034d483d26540f4e342d1b6f70f1f2f2e5a61
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992920"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationRubric = {
    displayName: 'Example Points Rubric',
    description: {
        content: 'This is an example of a rubric with points',
        contentType: 'text'
    },
    levels: [
        {
            displayName: 'Good',
            description: {
                content: '',
                contentType: 'text'
            },
            grading: {
                '@odata.type':'#microsoft.graph.educationAssignmentPointsGradeType',
                maxPoints: 2
            }
        },
        {
            displayName: 'Poor',
            description: {
                content: '',
                contentType: 'text'
            },
            grading: {
                '@odata.type':'#microsoft.graph.educationAssignmentPointsGradeType',
                maxPoints: 1
            }
        }
    ],
    qualities: [
        {
            description: {
                content: 'Argument',
                contentType: 'text'
            },
            criteria: [
                {
                    description: {
                        content: 'The essay\'s argument is persuasive.',
                        contentType: 'text'
                    }
                },
                {
                    description: {
                        content: 'The essay\'s argument does not make sense.',
                        contentType: 'text'
                    }
                }
            ],
            weight: 50.0
        },
        {
            description: {
                content: 'Spelling and Grammar',
                contentType: 'text'
            },
            criteria: [
                {
                    description: {
                        content: 'The essay uses proper spelling and grammar with few or no errors.',
                        contentType: 'text'
                    }
                },
                {
                    description: {
                        content: 'The essay has numerous errors in spelling and/or grammar.',
                        contentType: 'text'
                    }
                }
            ],
            weight: 50.0
        }
    ],
    grading: {
        '@odata.type':'#microsoft.graph.educationAssignmentPointsGradeType'
    }
};

await client.api('/education/me/rubrics')
    .post(educationRubric);

```