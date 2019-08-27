---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 312e339403f562294cb3c466ca884a82a3203cf6
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636703"
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
    .update(plannerPlanDetails);

```