---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 73440390b824f52c01bb04b7ac00181634d74f0d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791022"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerTask = {
  planId: 'xqQg5FS2LkCp935s-FIFm2QAFkHM',
  bucketId: 'hsOf2dhOJkqyYYZEtdzDe2QAIUCR',
  title: 'Update client list',
  assignments: {
    'fbab97d0-4932-4511-b675-204639209557': {
      '@odata.type': '#microsoft.graph.plannerAssignment',
      orderHint: ' !'
    }
  }
};

await client.api('/planner/tasks')
    .version('beta')
    .post(plannerTask);

```