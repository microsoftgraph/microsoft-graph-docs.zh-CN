---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22ce4fafb28ec1ae8dd9dc16941e4e3b19f04ab63d02defc2c65b38ea3e4bae7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333918"
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
    .post(plannerTask);

```