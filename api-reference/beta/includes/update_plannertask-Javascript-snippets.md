---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a46e6ad60a5c16de0c2281c85bb2bd7fb30c570a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480377"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerTask = {
  assignments: {
    fbab97d0-4932-4511-b675-204639209557: {
      @odata.type: "#microsoft.graph.plannerAssignment",
      orderHint: "N9917 U2883!"
    }
  },
  appliedCategories: {
    category3: true,
    category4: false
  }
};

let res = await client.api('/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh')
    .version('beta')
    .update({plannerTask : plannerTask});

```