---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fc49663e6b4df0a707a1b283db2b1e8a01062775
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636656"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerTask = {
  planId: "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  bucketId: "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  title: "Update client list",
  assignments: {
    fbab97d0-4932-4511-b675-204639209557: {
      @odata.type: "#microsoft.graph.plannerAssignment",
      orderHint: " !"
    }
  },
};

let res = await client.api('/planner/tasks')
    .version('beta')
    .post(plannerTask);

```