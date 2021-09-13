---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7a341da25cd4a39bb17039056cf4f50285c8b2ccaab4bd0ea7922328192a46a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107000"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerTask = {
  assignments: {
    'fbab97d0-4932-4511-b675-204639209557': {
      '@odata.type': '#microsoft.graph.plannerAssignment',
      orderHint: 'N9917 U2883!'
    }
  },
  appliedCategories: {
    category3: true,
    category4: false
  }
};

await client.api('/planner/tasks/{task-id}')
    .update(plannerTask);

```