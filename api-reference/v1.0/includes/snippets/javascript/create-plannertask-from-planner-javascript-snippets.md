---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dcb73dbad0cb26db55a18b38f897d3f4f16f438e
ms.sourcegitcommit: 9b507499fb1ec61b4de47f36f915ae29c8594459
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2020
ms.locfileid: "43935183"
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
  }
};

let res = await client.api('/planner/tasks')
    .post(plannerTask);

```