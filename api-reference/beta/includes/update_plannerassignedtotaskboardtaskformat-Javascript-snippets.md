---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3a2f6265cdfe6978aef95cac6e5f15fc8d8b2e6f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451270"
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

let res = await client.api('/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/assignedToTaskBoardFormat')
    .version('beta')
    .update({plannerAssignedToTaskBoardTaskFormat : plannerAssignedToTaskBoardTaskFormat});

```