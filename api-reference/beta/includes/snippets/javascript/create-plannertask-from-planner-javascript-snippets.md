---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5308f295a806be222ab91df73e43c4ca59623d9c8b94c2d414086c2b66213a8b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162462"
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