---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4cd41c929bd3126a2f60758dda184a596898f371
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722954"
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
    .post({plannerTask : plannerTask});

```