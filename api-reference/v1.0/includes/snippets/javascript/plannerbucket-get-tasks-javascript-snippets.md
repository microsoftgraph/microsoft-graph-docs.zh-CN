---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31288720573c8e937ba067a5152fb3d6994c3b9a
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "37637860"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/buckets/{task-id}/tasks')
    .get();

```