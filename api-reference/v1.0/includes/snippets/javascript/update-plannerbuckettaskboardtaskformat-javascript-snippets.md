---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 662e0930e99feeecedaecb7beda00629d6108241dd58c204a8cf09df536f2392
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409012"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerBucketTaskBoardTaskFormat = {
  orderHint: 'A6673H Ejkl!'
};

await client.api('/planner/tasks/{task-id}/bucketTaskBoardFormat')
    .update(plannerBucketTaskBoardTaskFormat);

```