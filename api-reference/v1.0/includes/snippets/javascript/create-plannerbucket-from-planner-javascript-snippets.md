---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3b4a1911300ba7a62a860f19530c50d6b6c30b2c7a59ba760779803b0a64dca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158695"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerBucket = {
  name: 'Advertising',
  planId: 'xqQg5FS2LkCp935s-FIFm2QAFkHM',
  orderHint: ' !'
};

await client.api('/planner/buckets')
    .post(plannerBucket);

```