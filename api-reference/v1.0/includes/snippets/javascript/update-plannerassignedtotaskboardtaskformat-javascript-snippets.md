---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3ab3af58ea169327e4c8f8cab40419dd11e9e124
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467823"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerAssignedToTaskBoardTaskFormat = {
  orderHintsByAssignee: {
    aaa27244-1db4-476a-a5cb-004607466324: "8566473P 957764Jk!"
  }
};

let res = await client.api('/planner/tasks/{task-id}/assignedToTaskBoardFormat')
    .update({plannerAssignedToTaskBoardTaskFormat : plannerAssignedToTaskBoardTaskFormat});

```