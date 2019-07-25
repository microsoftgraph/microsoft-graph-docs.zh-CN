---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8e7ea6f4a24763782310d51f1d879bbf2f161c5e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731772"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerBucketTaskBoardTaskFormat = {
  orderHint: "A6673H Ejkl!"
};

let res = await client.api('/planner/tasks/{task-id}/bucketTaskBoardFormat')
    .update({plannerBucketTaskBoardTaskFormat : plannerBucketTaskBoardTaskFormat});

```