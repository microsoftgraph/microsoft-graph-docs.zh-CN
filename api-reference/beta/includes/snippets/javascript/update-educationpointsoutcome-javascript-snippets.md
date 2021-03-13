---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a5c7c00c44510ceae7a80506c2748fde5450656
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799924"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationOutcome = {
    '@odata.type':'#microsoft.graph.educationPointsOutcome',
    points: {
        '@odata.type':'#microsoft.graph.educationAssignmentPointsGrade',
        points: 85.0
    }
};

await client.api('/education/me/assignments/{id}/submissions/{id}/outcomes/{id}')
    .version('beta')
    .update(educationOutcome);

```