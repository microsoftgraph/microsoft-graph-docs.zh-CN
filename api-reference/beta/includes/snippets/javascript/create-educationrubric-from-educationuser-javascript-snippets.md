---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e920366cbea97f7e39071277222397f10cbdc2e8
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636511"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationRubric = {
    displayName:"Example Points Rubric",
    description:{
        content:"This is an example of a rubric with points",
        contentType:"text"
    },
    levels:[
        {
            displayName:"Good",
            description:{
                content:"",
                contentType:"text"
            },
            grading:{
                @odata.type:"#microsoft.graph.educationAssignmentPointsGradeType",
                maxPoints:2
            }
        },
        {
            displayName:"Poor",
            description:{
                content:"",
                contentType:"text"
            },
            grading:{
                @odata.type:"#microsoft.graph.educationAssignmentPointsGradeType",
                maxPoints:1
            }
        }
    ],
    qualities:[
        {
            description:{
                content:"Argument",
                contentType:"text"
            },
            criteria:[
                {
                    description:{
                        content:"The essay's argument is persuasive.",
                        contentType:"text"
                    }
                },
                {
                    description:{
                        content:"The essay's argument does not make sense.",
                        contentType:"text"
                    }
                }
            ],
            weight:50.0
        },
        {
            description:{
                content:"Spelling and Grammar",
                contentType:"text"
            },
            criteria:[
                {
                    description:{
                        content:"The essay uses proper spelling and grammar with few or no errors.",
                        contentType:"text"
                    }
                },
                {
                    description:{
                        content:"The essay has numerous errors in spelling and/or grammar.",
                        contentType:"text"
                    }
                }
            ],
            weight:50.0
        }
    ],
    grading:{
        @odata.type:"#microsoft.graph.educationAssignmentPointsGradeType"
    }
};

let res = await client.api('/education/me/rubrics')
    .version('beta')
    .post(educationRubric);

```