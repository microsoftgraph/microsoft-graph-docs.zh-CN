---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 281c793c6c566f63a6be54e80127de859710bda2
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636523"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationOutcome = {
    @odata.type:"#microsoft.graph.educationPointsOutcome",
    points:{
        @odata.type:"#microsoft.graph.educationAssignmentPointsGrade",
        points:85.0
    }
};

let res = await client.api('/education/me/assignments/{id}/submissions/{id}/outcomes/{id}')
    .version('beta')
    .update(educationOutcome);

```