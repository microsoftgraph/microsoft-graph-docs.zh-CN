---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 70788378a3c2a92d363341901c3171262bcba906
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499772"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerBucketTaskBoardTaskFormat = {
  orderHint: "A6673H Ejkl!"
};

let res = await client.api('/planner/tasks/hsOf2dhOJkqyYYZEtdzDe2QAIUCR/bucketTaskBoardFormat')
    .version('beta')
    .update({plannerBucketTaskBoardTaskFormat : plannerBucketTaskBoardTaskFormat});

```