---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e6bfdae9dfe0d224ce669d561fcdf25899f3bcaa
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636657"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerBucket = {
  name: "Advertising",
  planId: "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  orderHint: " !"
};

let res = await client.api('/planner/buckets')
    .version('beta')
    .post(plannerBucket);

```