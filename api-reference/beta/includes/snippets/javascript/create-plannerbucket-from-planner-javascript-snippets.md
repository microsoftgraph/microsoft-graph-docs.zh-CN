---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9684ac7eedaa9afe246fa48c7725a4560a6ec5ccb240af3f5ed3351f7e0f70e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328877"
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
    .version('beta')
    .post(plannerBucket);

```