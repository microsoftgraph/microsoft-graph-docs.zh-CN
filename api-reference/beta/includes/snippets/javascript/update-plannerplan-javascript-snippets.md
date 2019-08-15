---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a798c73f389cb2948e29ad02a937c309f876814f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413261"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerPlan = {
  title: "title-value"
};

let res = await client.api('/planner/plans/{id}')
    .version('beta')
    .update({plannerPlan : plannerPlan});

```