---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8eb5ca7ad846b7a1f0481c0e37d44ddde98a7eee
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795538"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerBucket = {
  name: 'Development'
};

await client.api('/planner/buckets/{bucket-id}')
    .update(plannerBucket);

```