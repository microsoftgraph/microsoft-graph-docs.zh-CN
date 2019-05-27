---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 38bbfd75983205ef37fab8b039e5d3be63401174
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465097"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerPlanDetails = {
  sharedWith: {
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true,
    "d95e6152-f683-4d78-9ff5-67ad180fea4a" : false,
  },
  categoryDescriptions: {
    category1: "Indoors",
    category3: null,
  }
};

let res = await client.api('/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details')
    .version('beta')
    .update({plannerPlanDetails : plannerPlanDetails});

```